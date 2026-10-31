# Awesome-Cloud-Workload-Protection-Platform-CWPP

# Awesome-Cloud-Workload-Protection-Platform-CWPP

**Top Cloud Workload Protection Platform CWPP (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Runtime Protection, Container Security, Serverless Defense & Self-Hosted Workload Security*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Workload Protection Platforms (CWPP)**. These tools enable organizations to secure virtual machines, containers, Kubernetes clusters, and serverless functions at runtime—detecting and blocking threats like ransomware, cryptojacking, container escapes, and fileless attacks—from fully managed platforms with AI-driven behavioral analytics to self-hosted runtime engines built on open-source foundations like Falco.



**Examples** include CrowdStrike Falcon CWP, Prisma Cloud Compute, Wiz, SentinelOne Singularity Cloud, Sysdig Secure, Trend Micro Cloud One, Microsoft Defender for Servers, Aqua Security, Lacework FortiCNAPP, and Tenable Cloud Workload Protection (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted runtime security, container protection, and open workload defense. **Critical note**: The open-source CWPP landscape is anchored by **Falco**—the CNCF-graduated runtime engine that powers Sysdig Secure and serves as the de facto standard for container threat detection . **Tetragon** and **Tracee** offer eBPF-native alternatives with different enforcement models. **container-runtime-security** is the most feature-complete enforcement project. No open-source project matches CrowdStrike's AI-driven behavioral analytics or Prisma Cloud's full-lifecycle Defenders, but for runtime detection and enforcement, the open-source options are production-proven.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Cloud Workload Protection Platform (CWPP) market is estimated at approximately **$5.7B to $10.3B** (projected to reach over $30B by the early 2030s at an aggressive ~20–23% CAGR), driven by multi-cloud expansion, containerized microservices, and serverless architectures. The sector is **moderately fragmented and intensely competitive** rather than a winner-take-all market, marked by consolidation into CNAPP suites where hyperscalers (like Microsoft Defender for Cloud), pure-play cloud security pioneers (such as Wiz and Aqua Security), and enterprise cybersecurity incumbents (Palo Alto Networks, CrowdStrike, SentinelOne) vie for market share alongside an active open-source ecosystem.

## SaaS/Hosted Platforms

| Company Size (Revenue / Valuation) | Product / Platform | Pricing (Specific Starting Tiers) | Free Tier / Trial Limits | Key Capabilities & Trade-offs |
| :--- | :--- | :--- | :--- | :--- |
| **~$3.0T Market Cap** / ~$245B Ann. Rev. | **[Microsoft Defender for Servers](https://azure.microsoft.com/en-us/products/defender-for-cloud)** | **Plan 1**: ~$0.0067/server/hr (~$4.91/server/mo); **Plan 2**: ~$0.020/server/hr (~$14.60/server/mo) billed on active server uptime. | **30-day free trial** per plan with full features; foundational CSPM is permanently free. | Host & container protection across Azure, AWS, GCP & on-prem. Plan 2 required for agentless network-layer detection. |
| **~$110B Market Cap** / ~$8.0B Ann. Rev. | **[Prisma Cloud Compute](https://www.paloaltonetworks.com/prisma/cloud)** (Palo Alto Networks) | Credit-based licensing; modular entry configurations starting at **~$18,000/year** (CSPM) to **~$45,000/year** (full CNAPP suite). | **30-day free trial / PoC** via AWS Marketplace and direct sales; no permanent free tier. | Comprehensive host, container, and serverless runtime protection; available as SaaS (Enterprise) or self-hosted/air-gapped (Compute). |
| **~$80B Market Cap** / ~$4.0B Ann. Rev. | **[CrowdStrike Falcon Cloud Workload Protection](https://www.crowdstrike.com/)** | Flex licensing starts at **~$233.99/year** per host/workload license (via CDW); enterprise bundles quote-based. | **15-day free trial** with full cloud runtime detection and response access; no permanent free tier. | Unified agent-based breach prevention across VMs, containers, and K8s; requires Falcon platform base. |
| **~$55B Market Cap** / ~$5.5B Ann. Rev. | **[Lacework FortiCNAPP](https://www.lacework.com/)** (Fortinet) | Entry software licenses & starter deployment bundles starting at **~$22,000/year**; custom private offers via AWS Marketplace. | **30-day free trial** via AWS Marketplace and Fortinet portal; no permanent free tier. | AI-driven behavioral anomaly detection and Polygraph correlation uniting CWPP, CSPM, and CIEM; post-acquisition Fortinet integration. |
| **~$15B Market Cap** / ~$1.7B Ann. Rev. | **[SentinelOne Singularity Cloud Workload Security](https://www.sentinelone.com/)** | Cloud workload protection benchmarked starting at **~$36.00/VM/month** (~$432/VM/year); custom contract private offers on AWS Marketplace. | **30-day free evaluation / PoC** available through enterprise request; no permanent free tier. | Autonomous runtime protection and active rollback for servers, VMs, and Kubernetes against ransomware and fileless exploits. |
| **~$12B Valuation** (Private) / ~$500M+ ARR | **[Wiz Defend](https://www.wiz.io/)** | **Wiz Essential** starts at **$24,000/year** (min. 100 workloads @ $240/workload/yr); **Wiz Advanced** starts at **$38,000/year** (100 workloads). | **14-day free trial / PoC** with agentless visibility and Wiz Signals threat lake; no permanent free tier. | 100% agentless workload risk analysis complemented by lightweight Wiz Sensor runtime detection; high multi-cloud visibility. |
| **~$6.5B Market Cap** / ~$1.8B Ann. Rev. | **[Trend Micro Cloud One – Workload Security](https://www.trendmicro.com/)** | Hourly Pay-As-You-Go starts at **$0.007/instance/hr** (Essentials) up to **$0.011/instance/hr** (Medium/1 vCPU) and **$0.032/instance/hr** (Large). Annual licenses ~$385–$435/device. | **30-day free trial** with full protection-hours access on AWS Marketplace; no permanent free tier. | Mature runtime IPS/IDS, integrity monitoring, anti-malware, and container security with rich automation APIs. |
| **~$5.0B Market Cap** / ~$850M Ann. Rev. | **[Tenable Cloud Workload Protection](https://www.tenable.com/)** | Scoped per protected asset/resource, typically spanning **$28 to $90/asset/year** depending on volume; annual minimum contracts apply. | **Custom demo / scoped PoC** through sales; permanent free tier for standalone Nessus Essentials (limited to 16 IPs, vulnerability scanning only). | Scans virtual machines, container registries, and serverless functions for CVEs, secrets, and toxic combinations in multi-cloud assets. |
| **~$3.0B Valuation** (Private) / ~$300M+ ARR | **[Sysdig Secure](https://sysdig.com/)** | Node-based subscription starting at **$72.00 per host/month** (~$864/host/year) on AWS Marketplace (often with 20-host commitment tiers). | **30-day free trial** with full runtime policies; open-source Falco engine is **100% free forever** for self-hosting. | Built natively on CNCF Falco eBPF telemetry with 100+ out-of-the-box MITRE ATT&CK runtime rules and Kubernetes drift prevention. |
| **~$1.0B Valuation** (Private) / ~$100M+ ARR | **[Aqua Security](https://www.aquasec.com/)** | AWS Marketplace starting tiers: Shift Left Standard **$50,000/year**, Protect Advanced **$100,000/year**, and Ultimate **$150,000/year**. | **Custom 14- to 30-day guided PoC** on request; **Trivy open-source engine is 100% free forever** (unlimited scans). | Enterprise container, K8s, and AI workload runtime security with FedRAMP High authorization and granular supply chain controls. |

## Open-Source GitHub Projects



- **[Falco](https://github.com/falcosecurity/falco)**

  **Cloud-native runtime security** (Apache 2.0, CNCF Graduated) — **the de facto standard for container and Kubernetes runtime threat detection**, and the open-source engine powering Sysdig Secure's behavioral detections . **Features**: **eBPF-based** monitoring of system calls across hosts, containers, Kubernetes, and cloud services (via plugins for AWS CloudTrail, GitHub, Okta); **YAML rule engine** with out-of-the-box rules for container escapes, cryptojacking, reverse shells, privilege escalation, and fileless attacks; **100+ integrations** for forwarding alerts to SIEM, Slack, and data lakes; streaming detection minimizes storage costs. **Tech stack**: C++, Go. **Deploy**: Self-hosted (DaemonSet on Kubernetes, Helm chart). **Trade-off**: **Runtime detection only**—no posture management, vulnerability scanning, or CIEM. Requires rule tuning to avoid alert fatigue. **Best for**: teams needing runtime threat detection for Kubernetes and containers—the foundation of the runtime layer in any open-source CWPP stack.



- **[Tetragon](https://github.com/cilium/tetragon)**

  **eBPF-native runtime security and observability** (Apache 2.0) — **the enforcement-first alternative to Falco**, from Isovalent/Cilium. **Features**: **In-kernel enforcement** can kill processes before syscalls complete—not just alert after the fact; **Kubernetes-aware** process, file, and network visibility; **lower p99 CPU overhead** than Falco in some benchmarks; **TracingPolicy** CRDs for declarative security policies. **Tech stack**: Go, C (eBPF). **Deploy**: Self-hosted (DaemonSet on Kubernetes). **Trade-off**: **Smaller rule library than Falco**—fewer out-of-the-box detections; requires more custom policy authoring. **Best for**: teams wanting runtime enforcement (blocking, not just detecting) with eBPF-native performance—especially those already in the Cilium ecosystem.



- **[Tracee](https://github.com/aquasecurity/tracee)**

  **eBPF runtime security and forensics** (Apache 2.0) — **the forensic-focused runtime sensor** from Aqua Security. **Features**: **Built-in signature library** for common threats; **Rego policy support** for custom detection logic; **rich event context** for forensics and investigation; **Kubernetes and container awareness**; integrates with Aqua Platform. **Tech stack**: Go, C (eBPF). **Deploy**: Self-hosted (DaemonSet, CLI). **Trade-off**: **Runtime detection and forensics only**—no posture or vulnerability management. Smaller community than Falco. **Best for**: teams already in the Aqua ecosystem or wanting eBPF runtime detection with Rego-based policy customization.



- **[KubeArmor](https://github.com/kubearmor/KubeArmor)**

  **LSM-based runtime policy enforcement** (Apache 2.0) — **the policy-enforcement layer for container workloads**, using AppArmor, SELinux, and BPF-LSM. **Features**: **Enforcement at kernel LSM level**—blocks file, process, and network operations based on policy; **Kubernetes-native** with CRDs; **container and node-level policies**; integrates with observability tools. **Tech stack**: Go, C. **Deploy**: Self-hosted (DaemonSet). **Trade-off**: **Enforcement only**—no detection library or threat intelligence; you define the policies. **Best for**: teams needing to enforce least-privilege policies on container workloads at the kernel level—complements Falco's detection.



- **[container-runtime-security](https://github.com/aiagentmackenzie-lang/container-runtime-security)**

  **eBPF-based container runtime security monitoring and enforcement** (license per repo) — **the most feature-complete open-source runtime enforcement project** with AI triage. **Features**: **30 detection rules** across 9 categories (Container Escape, Cryptojacking, Reverse Shell, Credential Access, Privilege Escalation, Container Drift, Network Anomaly, Process Injection, Known CVE); **7-rule enforcement safety protocol** with TC-based network blocking; **multi-signal correlation** (shell→network, DNS+TLS); **AI triage** via gRPC (advisory); **~73k events/sec** single-core throughput. **Tech stack**: Go, C (eBPF). **Deploy**: Self-hosted (Kubernetes). **Trade-off**: **eBPF kernel load/attach path code-complete but pending Linux runtime verification** (Phase C); AI triage degrades to neutral. Newer project with limited community validation. **Best for**: teams wanting eBPF-native enforcement (not just detection) with AI-assisted triage—willing to validate the runtime path before production use.



- **[CWPP Design Studio](https://github.com/)**

  **Offline Streamlit application for CWPP lifecycle design** (open source, per LinkedIn author post) — **the most practical open-source reference architecture for CWPP programs**. **Features**: Walks through **build-time** (image/IaC scanning, secrets, SBOM), **ship-time** (registry scanning, Sigstore signing, admission control), **run-time** (process/file/network monitoring for VMs vs. containers vs. functions), **risk intelligence** (multi-factor prioritization beyond CVSS—exploitability + exposure + runtime reachability + data sensitivity), and **unified dashboard** correlating build-time findings with runtime context ("this vulnerable package is actually loaded in memory") . **Tech stack**: Python (Streamlit). **Deploy**: Local (offline, no API keys). **Trade-off**: **Design and assessment tool**—it does not perform runtime protection; it helps you design and evaluate a CWPP program . **Best for**: architects and security leads wanting a structured framework for designing or assessing their CWPP deployment—especially those building a program from scratch.



### Additional Strong Open-Source Options



- **Trivy** — Comprehensive scanner (Apache 2.0). Vulnerability, IaC, secrets, and SBOM scanning for images; CI/CD native. **Note**: Build-time scanner—pair with Falco for runtime. **Best for**: shift-left container security in CI/CD pipelines.

- **Kubescape** — Kubernetes security platform (Apache 2.0, CNCF incubating). Posture, vulnerability, and runtime for K8s clusters. **Note**: Kubernetes-only—not multi-cloud CWPP. **Best for**: teams wanting a single tool for Kubernetes workload security.

- **Kyverno** — Kubernetes admission controller (Apache 2.0). Policy enforcement via CRDs; signed-image verification via Sigstore. **Note**: Admission control only—not runtime detection. **Best for**: enforcing workload policies at the Kubernetes admission gate.



**Frameworks for building custom systems**: Combine **Falco** for runtime detection with **Tetragon** or **KubeArmor** for enforcement, **Trivy** for build-time scanning, and **CWPP Design Studio** as a reference architecture—creating a composable open-source CWPP stack. **None of these match CrowdStrike's AI-driven behavioral analytics or Prisma Cloud's full-lifecycle Defenders**, but for runtime detection and enforcement, the open-source options are production-proven.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- CWPP platforms handling workload credentials and runtime telemetry must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **The "runtime detection" vs. "runtime enforcement" vs. "build-time scanning" vs. "design framework" distinction is critical.** **Falco and Tracee** are **runtime detection**—they alert on threats but do not block them . **Tetragon and KubeArmor** are **runtime enforcement**—they block operations at the kernel or LSM level. **Trivy** is **build-time scanning**—it finds vulnerabilities before deployment. **CWPP Design Studio** is a **design framework**—it helps you architect a CWPP program but does not protect workloads . **Commercial platforms (CrowdStrike, Prisma Cloud, Wiz, SentinelOne, Sysdig, Trend Micro, Microsoft, Aqua, Lacework, Tenable)** bundle detection, enforcement, and scanning into unified products. **No single open-source project replaces a commercial CWPP.** Compose the stack based on your gaps.

- **Falco is the runtime detection standard**—CNCF Graduated, eBPF-based, and the open-source engine behind Sysdig Secure . **The trade-off**: detection only—no enforcement, no posture, no vulnerability scanning. **Pair it with Tetragon or KubeArmor for enforcement, and Trivy for build-time scanning.**

- **Tetragon's enforcement capability is a genuine differentiator**—it can kill processes before syscalls complete, not just alert after the fact. **The trade-off**: smaller rule library than Falco; requires more custom policy authoring. **For teams that need to block, not just detect, Tetragon is the strongest open-source option.**

- **Prisma Cloud Compute Edition is the only commercial CWPP with a self-hosted, air-gapped option**—it supports Projects for multi-tenancy and full data control . **If you need commercial-grade CWPP in an air-gapped environment, it is the option to evaluate.**

- **Wiz Defend's Agentless Workload Detection is uniquely valuable for unmonitorable assets**—virtual appliances, vendor-managed systems, and workloads that cannot run agents . **The trade-off**: agentless complements but does not fully replace agent-based runtime protection. **For teams with blind spots on appliances and gateways, it addresses a gap that pure agent-based tools cannot.**

- **Pricing opacity varies.** CrowdStrike publishes Flex licensing (~$233.99/year per license) . Aqua publishes AWS Marketplace tiers ($50K–$150K/year) . Trend Micro government edition is ~$385–$435 per device . Prisma Cloud, Wiz, SentinelOne, Sysdig, Microsoft, Lacework, and Tenable require sales contact or tiered estimation. **Validate with direct vendor conversations against your workload count and runtime requirements.**

- Self-hosted open-source solutions require proper infrastructure (Kubernetes for Falco/Tetragon, servers for management), security hardening for runtime sensors, and ongoing maintenance. **Runtime security tools have deep kernel-level visibility**—ensure your deployment meets your organization's security and performance requirements before deploying to production workloads.



---



**Made for cloud security engineers, platform teams, and organizations building transparent workload protection solutions.**

Let's make Cloud Workload Protection more open, data-driven, and runtime-aware.
