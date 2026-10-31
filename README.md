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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon Cloud Workload Protection](https://www.crowdstrike.com/)**

  **Comprehensive breach protection** across private, public, hybrid, and multi-cloud environments. Falcon CWP provides runtime protection for containers and Kubernetes alongside image assessment and CDR capabilities . **Pricing**: Flex licensing available (~$233.99/year for a single license per CDW listing) ; enterprise bundles quote-based. **Free tier**: None. **Best for**: CrowdStrike customers wanting workload protection integrated with endpoint and identity security—**trade-off**: workload protection is a module requiring appropriate Falcon tier.



- **[Prisma Cloud Compute](https://www.paloaltonetworks.com/prisma/cloud)** (Palo Alto Networks)

  **CWPP delivered as part of Prisma Cloud** (formerly Twistlock). Protects hosts, containers, and serverless across any cloud or datacenter. **Two editions**: **Enterprise Edition** (SaaS, Palo Alto manages Console) and **Compute Edition** (self-hosted, air-gapped support, Projects for multi-tenancy) . **Pricing**: Per-workload licensing; identical across editions. **Free tier**: None. **Best for**: enterprises wanting a single platform for CSPM and CWPP—**note**: Compute Edition is the choice for air-gapped or full-data-control environments .



- **[Wiz Defend](https://www.wiz.io/)**

  **Agentless cloud detection and response** extending Wiz's visibility to runtime threat detection. **Agentless Workload Detection** collects local logs from appliances (firewalls, gateways) that cannot run agents, correlating them with control plane events and Wiz Sensor runtime signals in the Wiz Signals data lake . **Pricing**: Quote-only. **Free tier**: None. **Best for**: Wiz customers wanting workload threat detection without agent deployment on every asset—**trade-off**: agentless detection complements but does not fully replace agent-based runtime protection for all workloads.



- **[SentinelOne Singularity Cloud Workload Security](https://www.sentinelone.com/)**

  **AI-driven runtime protection** for servers, VMs, and containers across on-premises, private cloud, and public clouds. Blocks ransomware, cryptojacking, and fileless attacks at execution with autonomous response at the workload level . **Pricing**: Quote-only; endpoint-based pricing models available. **Free tier**: None. **Best for**: organizations wanting autonomous runtime protection with AI-driven detection—**trade-off**: full CNAPP scope may require additional SentinelOne modules.



- **[Sysdig Secure](https://sysdig.com/)**

  **CNAPP built on open-source Falco** with deep system call visibility for runtime threat detection. Core built on Falco, sysdig OSS, and Cloud Custodian; unified security and monitoring; 100+ out-of-the-box runtime policies with MITRE ATT&CK mapping; serverless container support including inline Fargate scanning . **Pricing**: Simple node-based pricing (per protected node) . **Free tier**: Falco OSS is free. **Best for**: Kubernetes-heavy environments wanting Falco-native runtime security with commercial support—**trade-off**: agent deployment required for runtime; node-based pricing scales with cluster size .



- **[Trend Micro Cloud One – Workload Security](https://www.trendmicro.com/)**

  **Comprehensive detection and protection** purpose-built for server, cloud, and container environments with consistent security regardless of workload type. Rich API set for automation . **Pricing**: Subscription licensing (~$385–$435 per device for government edition per CDW-G listing) ; commercial quote-based. **Free tier**: None. **Best for**: organizations wanting workload security across hybrid environments with automation-friendly APIs.



- **[Microsoft Defender for Servers](https://azure.microsoft.com/en-us/products/defender-for-cloud)**

  **Threat detection and advanced protection** for Windows and Linux machines across Azure, AWS, GCP, and on-premises. **Plan 1** deploys Defender for Endpoint with hourly billing (cost-effective for intermittent VMs); **Plan 2** adds agentless network-layer threat detection and full server features . **Pricing**: Plan 1 per-hour; Plan 2 per-server. **Free tier**: None for workload protection. **Best for**: Microsoft-centric organizations wanting native server protection across multi-cloud—**trade-off**: Plan 2 required for agentless network detection.



- **[Aqua Security](https://www.aquasec.com/)**

  **Full-lifecycle CNAPP** securing containers, serverless, Kubernetes, and AI workloads. FedRAMP High Authorized; runtime protection detects threats and enforces compliance across cloud-native workloads; purpose-built AI workload security for LLM governance and model abuse detection . **Pricing**: AWS Marketplace tiers: Shift Left Standard **$50,000/year**; Protect Advanced **$100,000/year**; Ultimate **$150,000/year** . **Free tier**: None. **Best for**: regulated enterprises needing FedRAMP-authorized container and Kubernetes security with AI workload coverage.



- **[Lacework FortiCNAPP](https://www.lacework.com/)** (Fortinet)

  **AI-driven behavioral analytics** unifying CWPP, CSPM, and CIEM. SC Award 2025 winner for Best Cloud Workload Protection Solution. Correlates signals into composite alerts; agent-based and agentless deployment; customers report **75% reduction in compliance violations**, **100:1 alert-to-noise ratio**, and **80% faster investigations** . **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations wanting behavioral anomaly detection with consolidated CNAPP—**trade-off**: Fortinet ecosystem integration post-acquisition.



- **[Tenable Cloud Workload Protection](https://www.tenable.com/)**

  **CWPP within Tenable Cloud Security** scanning VMs, containers, and serverless functions for vulnerabilities, secrets, sensitive data, malware, and misconfigurations . **Pricing**: Quote-only. **Free tier**: None. **Best for**: Tenable customers wanting workload scanning integrated with broader exposure management.



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
