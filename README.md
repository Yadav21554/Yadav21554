<div align="center">

# 🚀 Sunny Yadav
### **Cloud DevSecOps Engineer & Agentic AI Infrastructure Architect**
*Specializing in Zero-Trust Cloud Platforms, Production GitOps, and Autonomous AI Agent Tooling (MCP & RAG)*

<br/>

<a href="https://github.com/Yadav21554">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&pause=1000&color=38BDF8&center=true&vCenter=true&width=700&lines=🛡️+Zero-Trust+Cloud+Architecture+%E2%80%A2+Azure+%26+AWS;🤖+Agentic+AI+Infrastructure+%E2%80%A2+Model+Context+Protocol+(MCP);☸️+Kubernetes+(AKS%2FEKS)+%E2%80%A2+Terraform+IaC+%E2%80%A2+GitOps;🔐+Shift-Left+Security+%E2%80%A2+Cosign+Signing+%E2%80%A2+Trivy+Gates;⚡+Production+RAG+Pipelines+%E2%80%A2+pgvector+%E2%80%A2+LLMOps" alt="Typing SVG" />
</a>

<br/>
<br/>

[![Open for Opportunities](https://img.shields.io/badge/STATUS-OPEN%20FOR%20HIRE-success?style=for-the-badge&logo=rocket&logoColor=white)](https://github.com/Yadav21554)
[![Specialization](https://img.shields.io/badge/ROLE-DEVSECOPS%20%2B%20AI%20INFRA-0284C7?style=for-the-badge&logo=azuredevops&logoColor=white)](https://github.com/Yadav21554)
[![Profile Views](https://komarev.com/ghpvc/?username=Yadav21554&label=PROFILE+VIEWS&color=8B5CF6&style=for-the-badge)](https://github.com/Yadav21554)

<br/>

<!-- Professional Social Links -->
<a href="https://www.linkedin.com/in/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
&nbsp;&nbsp;
<a href="mailto:sunnyyadav@example.com"><img src="https://img.shields.io/badge/Email-Get%20in%20Touch-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
&nbsp;&nbsp;
<a href="https://github.com/Yadav21554"><img src="https://img.shields.io/badge/GitHub-Follow%20Me-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>

</div>

---

## 👨‍💻 Professional Summary

I am a **Cloud DevSecOps Engineer & Agentic AI Specialist** with deep expertise in architecting resilient, zero-trust cloud infrastructure and next-generation cognitive systems. My focus is engineering production platforms that bridge **hyperscale cloud security (Azure / AWS / Kubernetes / Terraform)** with **modern AI agent infrastructure (Model Context Protocol [MCP], Hybrid RAG, and Multi-Agent Orchestration)**.

- 🛡️ **Zero-Trust Cloud Networking:** Expert in designing air-gapped Virtual Networks (VNets/VPCs), split-horizon DNS routing, Azure Private DNS Zones, and Private Link endpoints that eliminate public ingress surfaces.
- 🔐 **Shift-Left DevSecOps:** Experienced in integrating automated SAST/DAST/SCA security gates, container image signing (`cosign`), SBOM generation (`syft`), and policy-as-code (`kyverno`/`opa`) into CI/CD pipelines.
- 🤖 **Agentic AI & LLMOps:** Building custom Model Context Protocol (MCP) servers, sandboxed tool registries, and hybrid RAG pipelines (BM25 + pgvector) to enable autonomous, secure AI workflows for cloud operations.

---

## 🛠️ Technical Skills & Competencies

### ☁️ Cloud & Infrastructure as Code
- **Cloud Platforms:** Microsoft Azure (VNets, Private DNS, Private Endpoints, AKS, Bastion, ExpressRoute), AWS (VPC, Route53, EKS, IAM), Google Cloud Platform
- **Infrastructure as Code (IaC):** Terraform, OpenTofu, Terragrunt, Ansible, Packer
- **Containers & Orchestration:** Docker, Kubernetes (AKS/EKS), Helm Charts, Cilium eBPF, Istio Service Mesh

### 🛡️ DevSecOps & Security Engineering
- **Vulnerability & Compliance Scanning:** Trivy, Snyk, Checkov, SonarQube, tfsec
- **Software Supply Chain Security:** Cosign (Sigstore keyless signing), Syft (SBOM generation), SLSA Framework
- **Secrets Management & Policy:** HashiCorp Vault (dynamic secrets, AppRole), Kyverno, OPA / Gatekeeper
- **Runtime Security & Monitoring:** Falco, Prometheus, Grafana, OpenTelemetry, Azure Monitor

### 🤖 Agentic AI & Cognitive Infrastructure
- **Agent Protocols & Frameworks:** Model Context Protocol (MCP - stdio/SSE transports), LangGraph, CrewAI
- **Retrieval-Augmented Generation (RAG):** Hybrid Vector Search, Reciprocal Rank Fusion (RRF), pgvector, ChromaDB
- **LLM Security & Guardrails:** OWASP Top 10 for LLMs, Prompt Injection Defense, Pydantic Schema Validation

### 💻 Languages & Scripting
- **Core Languages:** Python 3.12 (FastAPI, FastMCP, AsyncIO), Bash/Shell scripting, PowerShell Core, SQL (PostgreSQL), HCL (Terraform)

---

## 💼 Featured Engineering Projects & Architectural Portfolio

### 1. 🛡️ Enterprise Zero-Trust Cloud Landing Zone (Azure & Terraform)
> **Domain:** Cloud Architecture • Zero-Trust Networking • Infrastructure as Code

- **Challenge:** Enterprise applications containing sensitive data (e.g., HR/Benefits portals, core databases) are frequently exposed to reconnaissance and DNS exfiltration when configured with public endpoints or misconfigured DNS.
- **Architectural Solution:**
  - Designed an air-gapped **Hub-and-Spoke Azure VNet topology (`10.124.0.0/16`)** with dedicated subnet microsegmentation.
  - Implemented **Azure Private DNS Zones** integrated with Azure’s virtualized Wire Server (`168.63.129.16`) to provide deterministic internal domain resolution without public IP exposure.
  - Configured **Split-Horizon DNS** so external internet users resolve only reverse-proxy edge gateways, while internal virtual desktops (AVD) resolve private RFC 1918 backend addresses securely.
  - 100% codified using modular, reusable **Terraform HCL**.
- **Tech Stack:** `Azure Private DNS` • `Virtual Networks (VNets)` • `Terraform` • `Nginx` • `Azure Bastion`

---

### 2. 🤖 Sentinel-MCP: Autonomous DevSecOps Security Triage Agent
> **Domain:** Agentic AI • Model Context Protocol (MCP) • Vulnerability Management

- **Challenge:** DevSecOps teams face alert fatigue from hundreds of daily container vulnerability alerts and cloud drift notifications.
- **Architectural Solution:**
  - Engineered a custom **Model Context Protocol (MCP) Server** that exposes sandboxed security tools (`tools/list`, `tools/call`) via JSON-RPC 2.0.
  - Built an autonomous multi-agent supervisor (using **LangGraph**) that ingests Trivy container CVE findings, cross-references internal compliance policies, and automatically drafts pull requests to remediate vulnerable dependencies.
  - Enforced strict least-privilege sandboxing: agents execute within read-only cluster scopes and require cryptographic signature verification (`cosign`) before committing fixes.
- **Tech Stack:** `Python (FastMCP)` • `Model Context Protocol` • `LangGraph` • `Trivy` • `Cosign` • `GitHub API`

---

### 3. ☸️ Production Hardened Kubernetes GitOps Pipeline
> **Domain:** Container Security • Supply Chain Integrity • GitOps

- **Challenge:** Preventing unverified, vulnerable container images from running in production Kubernetes clusters.
- **Architectural Solution:**
  - Built an end-to-end **GitHub Actions CI/CD pipeline** enforcing shift-left security gates (SAST with Semgrep, SCA with Snyk, and IaC scanning with Checkov).
  - Integrated **Cosign** for keyless cryptographic container image signing using GitHub OIDC identity.
  - Implemented **Kyverno admission controller policies** on AKS that intercept deployment requests and reject any image lacking a valid cryptographic signature or running as root.
  - Managed cluster deployments declaratively through **ArgoCD GitOps** with automated drift detection.
- **Tech Stack:** `Kubernetes (AKS)` • `ArgoCD` • `Cosign` • `Kyverno` • `Checkov` • `GitHub Actions`

---

### 4. ⚡ Cortex-RAG: Sub-Second Cloud Runbook Knowledge Engine
> **Domain:** Generative AI • Hybrid Vector Search • LLMOps

- **Challenge:** Cloud incident response is slowed down when on-call engineers must manually search through extensive, fragmented infrastructure runbooks and compliance documents.
- **Architectural Solution:**
  - Architected a **Production Hybrid RAG Pipeline** combining dense semantic embeddings (`pgvector`) with sparse lexical keyword matching (BM25) via PostgreSQL.
  - Implemented **Reciprocal Rank Fusion (RRF)** to accurately retrieve exact identifiers (CVE IDs, error codes, IP addresses) alongside conceptual context in under 85ms.
  - Added an output guardrail layer enforcing structured Pydantic schemas and preventing hallucinated command recommendations.
- **Tech Stack:** `Python` • `PostgreSQL / pgvector` • `FastAPI` • `LlamaIndex` • `BM25 Hybrid Search`

---

## 🏛️ Architecture Case Study: Enterprise Zero-Trust DNS Resolution

To eliminate the attack surface of internal corporate workloads, I design private resolution topologies that separate public internet discovery from authenticated corporate access:

### 1. Split-Horizon DNS Architecture
- **Public Query Path:** External requests (`dashboard.company.com`) route through public authoritative name servers to public edge ingress points (DMZ).
- **Private Query Path:** Internal requests (`portal.company.internal`) route exclusively within the private VNet through Azure’s Wire Server (`168.63.129.16`), resolving to internal private RFC 1918 IPs (`10.124.0.4`).
- **Result:** Backend application servers operate with **zero public IP addresses**, rendering internal topologies invisible to external port scanners and adversaries.

### 2. Client Resolution Hierarchy
All operating systems adhere to a strict resolution hierarchy that must be considered during cloud networking design:
1. **Local Hosts File** (`/etc/hosts` or `C:\Windows\System32\drivers\etc\hosts`) — immediate override.
2. **Local OS Resolver Cache** (`nscd`, `systemd-resolved`, or Windows DNS cache).
3. **Configured Recursive Wire Server** (`168.63.129.16:53`) — hypervisor-level routing that evaluates linked Private DNS Zones before external recursion.

---

## 🤖 Why I Build with Model Context Protocol (MCP) & AI Agents

The future of cloud operations is autonomous, but autonomy without boundaries is dangerous:

> **"Model Context Protocol (MCP) is the missing security and integration layer for enterprise AI. It replaces unsafe, ad-hoc shell access with structured, typed JSON-RPC contracts and role-based tool authorization."**

By combining **MCP tool sandboxes**, **Hybrid RAG knowledge retrieval**, and **Multi-Agent State Machines (LangGraph)**, I build AI systems that can:
- Autonomously analyze Kubernetes pod crash loops and network partition logs.
- Map CVE vulnerabilities to exact enterprise remediation runbooks.
- Propose signed, tested Terraform code changes without human bottlenecking.

---

## 📈 GitHub Telemetry & Real-Time Stats

<div align="center">
  <table border="0">
    <tr>
      <td align="center" width="50%">
        <img src="https://github-readme-stats.vercel.app/api?username=Yadav21554&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=38BDF8&text_color=94A3B8&icon_color=38BDF8&count_private=true" width="100%" alt="Sunny's GitHub Stats" />
      </td>
      <td align="center" width="50%">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Yadav21554&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=38BDF8&text_color=94A3B8" width="100%" alt="Top Languages" />
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center" width="100%">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Yadav21554&theme=tokyonight&hide_border=true&background=0D1117&ring=38BDF8&fire=F59E0B&currStreakLabel=38BDF8" width="80%" alt="GitHub Streak" />
      </td>
    </tr>
  </table>
</div>

---

## 🎯 Continuous Learning & Professional Tenets

- **Zero-Trust by Default:** Never trust the network perimeter; verify explicitly, enforce least-privilege RBAC, and air-gap sensitive workloads.
- **Everything as Code (EaC):** If infrastructure, security policies, or agent tool schemas are not stored in Git, they do not exist in production.
- **Shift-Left Security:** Catch vulnerabilities, misconfigurations, and drift at the commit gate—never after a breach in production.
- **Relentless Growth:** *"Consistent learning is painful, but mandatory. To build world-class systems, one must become an extraordinary learner."*

---

## 📬 Let's Connect & Collaborate

I am actively open to discussing **DevSecOps Engineer, Cloud Architect, and AI Infrastructure** roles, as well as collaborative open-source cloud projects:

<div align="center">

<a href="https://www.linkedin.com/in/">
  <img src="https://img.shields.io/badge/LinkedIn-Connect%20with%20Sunny-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="mailto:sunnyyadav@example.com">
  <img src="https://img.shields.io/badge/Email-Direct%20Inquiry-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com/Yadav21554">
  <img src="https://img.shields.io/badge/GitHub-Follow%20%40Yadav21554-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>

<br/><br/>

<sub>Designed and engineered as a professional digital resume by <b>Sunny Yadav</b>.</sub>

</div>
