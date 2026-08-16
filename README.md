# Awesome Cybersecurity Blue Team with stars

> A collection of awesome resources, tools, and other shiny things for cybersecurity blue teams.

[Cybersecurity blue teams](https://en.wikipedia.org/wiki/Blue_team_\(computer_security\)) are groups of individuals who identify security flaws in information technology systems, verify the effectiveness of security measures, and monitor the systems to ensure that implemented defensive measures remain effective in the future. While not exclusive, this list is heavily biased towards [Free Software](https://www.gnu.org/philosophy/free-sw.html) projects and against proprietary products or corporate services. For offensive TTPs, please see [awesome-pentest](https://github.com/fabacab/awesome-pentest) ⭐ 280 | 🐛 0 | 📅 2023-10-23.

Your contributions and suggestions are heartily ♥ welcome. (✿◕‿◕). Please check the [Contributing Guidelines](CONTRIBUTING.md) for more details. This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

Many cybersecurity professionals enable racist state violence, wittingly or unwittingly, by providing services to local, state, and federal policing agencies or otherwise cooperating with similar institutions who do so. This evil most often happens through the coercive mechanism of employment under threat of lack of access to food, shelter, or healthcare. Despite this list's public availability, it is the maintainer's intention and hope that this list supports the people and organizations who work to counter such massive albeit banal evil.

![Image of a raised fist composed of the names of Black people murdered by taxpayer-funded racist police violence.](https://web.archive.org/web/20201028021653if_/https://lauerrealtygroup.com/wp-content/uploads/2020/06/BLM-FIST-scaled.jpg)

![Image of a "Blue Lives Matter" flag with the thin blue line being peeled away to reveal a Nazi swastika underneath.](https://web.archive.org/web/20201123181815if_/https://i.redd.it/86pl28p0dl631.jpg)

**[DEFUND THE POLICE.](https://defundthepolice.org/)**

## Contents

* [Automation and Convention](#automation-and-convention)
  * [Code libraries and bindings](#code-libraries-and-bindings)
  * [Security Orchestration, Automation, and Response (SOAR)](#security-orchestration-automation-and-response-soar)
* [Cloud platform security](#cloud-platform-security)
  * [Distributed monitoring](#distributed-monitoring)
  * [Kubernetes](#kubernetes)
  * [Service meshes](#service-meshes)
* [Communications security (COMSEC)](#communications-security-comsec)
* [DevSecOps](#devsecops)
  * [Application or Binary Hardening](#application-or-binary-hardening)
  * [Compliance testing and reporting](#compliance-testing-and-reporting)
  * [Dependency confusion](#dependency-confusion)
  * [Fuzzing](#fuzzing)
  * [Policy enforcement](#policy-enforcement)
  * [Supply chain security](#supply-chain-security)
* [Honeypots](#honeypots)
  * [Tarpits](#tarpits)
* [Host-based tools](#host-based-tools)
  * [Sandboxes](#sandboxes)
* [Identity and AuthN/AuthZ](#identity-and-authnauthz)
* [Incident Response tools](#incident-response-tools)
  * [IR management consoles](#ir-management-consoles)
  * [Evidence collection](#evidence-collection)
* [Network perimeter defenses](#network-perimeter-defenses)
  * [Firewall appliances or distributions](#firewall-appliances-or-distributions)
* [Operating System distributions](#operating-system-distributions)
* [Phishing awareness and reporting](#phishing-awareness-and-reporting)
* [Preparedness training and wargaming](#preparedness-training-and-wargaming)
  * [Post-engagement analysis and reporting](#post-engagement-analysis-and-reporting)
* [Security configurations](#security-configurations)
* [Security monitoring](#security-monitoring)
  * [Endpoint Detection and Response (EDR)](#endpoint-detection-and-response-edr)
  * [Network Security Monitoring (NSM)](#network-security-monitoring-nsm)
  * [Security Information and Event Management (SIEM)](#security-information-and-event-management-siem)
  * [Service and performance monitoring](#service-and-performance-monitoring)
  * [Threat hunting](#threat-hunting)
* [Threat intelligence](#threat-intelligence)
  * [Fingerprinting](#fingerprinting)
  * [Threat signature packages and collections](#threat-signature-packages-and-collections)
* [Tor Onion service defenses](#tor-onion-service-defenses)
* [Transport-layer defenses](#transport-layer-defenses)
  * [Overlay and Virtual Private Networks (VPNs)](#overlay-and-virtual-private-networks-vpns)
* [macOS-based defenses](#macos-based-defenses)
* [Windows-based defenses](#windows-based-defenses)
  * [Active Directory](#active-directory)

## Automation and Convention

* [DShell](https://github.com/USArmyResearchLab/Dshell) ⭐ 5,490 | 🐛 4 | 🌐 Python | 📅 2024-05-07 - Extensible network forensic analysis framework written in Python that enables rapid development of plugins to support the dissection of network packet captures.
* [Password Manager Resources](https://github.com/apple/password-manager-resources) ⭐ 4,784 | 🐛 131 | 🌐 JavaScript | 📅 2026-08-13 - Collaborative, crowd-sourced data and code to make password management better.
* [Clevis](https://github.com/latchset/clevis) ⭐ 1,243 | 🐛 159 | 🌐 Shell | 📅 2026-07-25 - Plugable framework for automated decryption, often used as a Tang client.
* [Ansible Lockdown](https://ansiblelockdown.io/) - Curated collection of information security themed Ansible roles that are both vetted and actively maintained.
* [Dev-Sec.io](https://dev-sec.io/) - Server hardening framework providing Ansible, Chef, and Puppet implementations of various baseline security configurations.
* [peepdf](https://eternal-todo.com/tools/peepdf-pdf-analysis-tool) - Scriptable PDF file analyzer.
* [PyREBox](https://talosintelligence.com/pyrebox) - Python-scriptable reverse engineering sandbox, based on QEMU.
* [Watchtower](https://containrrr.dev/watchtower/) - Container-based solution for automating Docker container base image updates, providing an unattended upgrade experience.

### Code libraries and bindings

* [MultiScanner](https://github.com/mitre/multiscanner) ⭐ 620 | 🐛 39 | 🌐 Python | 📅 2019-10-08 - File analysis framework written in Python that assists in evaluating a set of files by automatically running a suite of tools against them and aggregating the output.
* [censys-python](https://github.com/censys/censys-python) ⭐ 468 | 🐛 5 | 🌐 Python | 📅 2026-07-26 - Python wrapper to the Censys REST API.
* [python-stix2](https://github.com/oasis-open/cti-python-stix2) ⭐ 434 | 🐛 67 | 🌐 Python | 📅 2026-02-12 - Python APIs for serializing and de-serializing Structured Threat Information eXpression (STIX) JSON content, plus higher-level APIs for common tasks.
* [libcrafter](https://github.com/pellegre/libcrafter) ⭐ 312 | 🐛 4 | 🌐 Rust | 📅 2026-08-16 - High level C++ network packet sniffing and crafting library.
* [python-sandboxapi](https://github.com/InQuest/python-sandboxapi) ⭐ 143 | 🐛 0 | 🌐 Python | 📅 2024-01-31 - Minimal, consistent Python API for building integrations with malware sandboxes.
* [Posh-VirusTotal](https://github.com/darkoperator/Posh-VirusTotal) ⭐ 124 | 🐛 7 | 🌐 PowerShell | 📅 2020-01-16 - PowerShell interface to VirusTotal.com APIs.
* [python-dshield](https://github.com/rshipp/python-dshield) ⭐ 28 | 🐛 1 | 🌐 Python | 📅 2023-05-23 - Pythonic interface to the Internet Storm Center/DShield API.

### Security Orchestration, Automation, and Response (SOAR)

See also [Security Information and Event Management (SIEM)](#security-information-and-event-management-siem), and [IR management consoles](#ir-management-consoles).

* [Shuffle](https://shuffler.io/) - Graphical generalized workflow (automation) builder for IT professionals and blue teamers.

## Cloud platform security

See also [asecure.cloud/tools](https://asecure.cloud/tools/).

* [gVisor](https://github.com/google/gvisor) ⭐ 19,094 | 🐛 779 | 🌐 Go | 📅 2026-08-15 - Application kernel, written in Go, that implements a substantial portion of the Linux system surface to provide an isolation boundary between the application and the host kernel.
* [Prowler](https://github.com/toniblyx/prowler) ⭐ 14,592 | 🐛 275 | 🌐 Python | 📅 2026-08-14 - Tool based on AWS-CLI commands for Amazon Web Services account security assessment and hardening.
* [Scout Suite](https://github.com/nccgroup/ScoutSuite) ⭐ 7,789 | 🐛 295 | 🌐 Python | 📅 2025-09-23 - Open source multi-cloud security-auditing tool, which enables security posture assessment of cloud environments.
* [Principal Mapper (PMapper)](https://github.com/nccgroup/PMapper) ⭐ 1,574 | 🐛 36 | 🌐 Python | 📅 2024-08-02 - Quickly evaluate IAM permissions in AWS via script and library capable of identifying risks in the configuration of AWS Identity and Access Management (IAM) for an AWS account or an AWS organization.
* [Aaia](https://github.com/rams3sh/Aaia) ⭐ 296 | 🐛 4 | 🌐 Python | 📅 2026-01-23 - Helps in visualizing AWS IAM and Organizations in a graph format with help of Neo4j.
* [Falco](https://falco.org/) - Behavioral activity monitor designed to detect anomalous activity in containerized applications, hosts, and network packet flows by auditing the Linux kernel and enriched by runtime data such as Kubernetes metrics.
* [Kata Containers](https://katacontainers.io/) - Secure container runtime with lightweight virtual machines that feel and perform like containers, but provide stronger workload isolation using hardware virtualization technology as a second layer of defense.

### Distributed monitoring

See also [§ Service and performance monitoring](#service-and-performance-monitoring).

* [Cortex](https://cortexmetrics.io/) - Provides horizontally scalable, highly available, multi-tenant, long term storage for Prometheus.
* [Jaeger](https://www.jaegertracing.io/) - Distributed tracing platform backend used for monitoring and troubleshooting microservices-based distributed systems.
* [OpenTelemetry](https://opentelemetry.io/) - Observability framework for cloud-native software, comprising a collection of tools, APIs, and SDKs for exporting application performance metrics to a tracing backend (formerly maintained by the OpenTracing and OpenCensus projects).
* [Prometheus](https://prometheus.io/) - Open-source systems monitoring and alerting toolkit originally built at SoundCloud.
* [Zipkin](https://zipkin.io/) - Distributed tracing system backend that helps gather timing data needed to troubleshoot latency problems in service architectures.

### Kubernetes

See also [Kubernetes-Security.info](https://kubernetes-security.info/).

* [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets) ⭐ 9,246 | 🐛 73 | 🌐 Go | 📅 2026-08-11 - Kubernetes controller and tool for one-way encrypted Secrets.
* [kubernetes-event-exporter](https://github.com/opsgenie/kubernetes-event-exporter) ⚠️ Archived - Allows exporting the often missed Kubernetes events to various outputs so that they can be used for observability or alerting purposes.
* [k-rail](https://github.com/cruise-automation/k-rail) ⚠️ Archived - Workload policy enforcement tool for Kubernetes.
* [Managed Kubernetes Inspection Tool (MKIT)](https://github.com/darkbitio/mkit) ⚠️ Archived - Query and validate several common security-related configuration settings of managed Kubernetes cluster objects and the workloads/resources running inside the cluster.
* [kube-forensics](https://github.com/keikoproj/kube-forensics) ⭐ 234 | 🐛 25 | 🌐 Go | 📅 2026-07-16 - Allows a cluster administrator to dump the current state of a running pod and all its containers so that security professionals can perform off-line forensic analysis.
* [certificate-expiry-monitor](https://github.com/muxinc/certificate-expiry-monitor) ⭐ 169 | 🐛 3 | 🌐 Go | 📅 2022-06-08 - Utility that exposes the expiry of TLS certificates as Prometheus metrics.
* [KubeSec](https://kubesec.io/) - Static analyzer of Kubernetes manifests that can be run locally, as a Kuberenetes admission controller, or as its own cloud service.
* [Kyverno](https://kyverno.io/) - Policy engine designed for Kubernetes.
* [Linkerd](https://linkerd.io/) - Ultra light Kubernetes-specific service mesh that adds observability, reliability, and security to Kubernetes applications without requiring any modification of the application itself.
* [Polaris](https://polaris.docs.fairwinds.com/) - Validates Kubernetes best practices by running tests against code commits, a Kubernetes admission request, or live resources already running in a cluster.
* [kube-hunter](https://kube-hunter.aquasec.com/) - Open-source tool that runs a set of tests ("hunters") for security issues in Kubernetes clusters from either outside ("attacker's view") or inside a cluster.

### Service meshes

See also [ServiceMesh.es](https://servicemesh.es/).

* [Consul](https://consul.io/) - Solution to connect and configure applications across dynamic, distributed infrastructure and, with Consul Connect, enabling secure service-to-service communication with automatic TLS encryption and identity-based authorization.
* [Istio](https://istio.io/) - Open platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data.

## Communications security (COMSEC)

See also [Transport-layer defenses](#transport-layer-defenses).

* [GPG Sync](https://github.com/firstlookmedia/gpgsync) ⚠️ Archived - Centralize and automate OpenPGP public key distribution, revocation, and updates amongst all members of an organization or team.
* [Geneva (Genetic Evasion)](https://censorship.ai/) - Novel experimental genetic algorithm that evolves packet-manipulation-based censorship evasion strategies against nation-state level censors to increase availability of otherwise blocked content.
* [GlobaLeaks](https://www.globaleaks.org/) - Free, open source software enabling anyone to easily set up and maintain a secure whistleblowing platform.
* [SecureDrop](https://securedrop.org/) - Open source whistleblower submission system that media organizations and NGOs can install to securely accept documents from anonymous sources.
* [Teleport](https://goteleport.com/) - Allows engineers and security professionals to unify access for SSH servers, Kubernetes clusters, web applications, and databases across all environments.

## DevSecOps

See also [awesome-devsecops](https://github.com/devsecops/awesome-devsecops) ⭐ 5,455 | 🐛 77 | 📅 2024-05-11.

* [Trivy](https://github.com/aquasecurity/trivy) ⭐ 37,425 | 🐛 238 | 🌐 Go | 📅 2026-08-14 - Simple and comprehensive vulnerability scanner for containers and other artifacts, suitable for use in continuous integration pipelines.
* [SOPS](https://github.com/mozilla/sops) ⭐ 22,831 | 🐛 438 | 🌐 Go | 📅 2026-08-10 - Editor of encrypted files that supports YAML, JSON, ENV, INI and binary formats and encrypts with AWS KMS, GCP KMS, Azure Key Vault, and PGP.
* [Git Secrets](https://github.com/awslabs/git-secrets) ⭐ 13,371 | 🐛 131 | 🌐 Shell | 📅 2025-09-17 - Prevents you from committing passwords and other sensitive information to a git repository.
* [Clair](https://github.com/coreos/clair) ⭐ 11,047 | 🐛 59 | 🌐 Go | 📅 2026-08-11 - Static analysis tool to probe for vulnerabilities introduced via application container (e.g., Docker) images.
* [BlackBox](https://github.com/StackExchange/blackbox) ⚠️ Archived - Safely store secrets in Git/Mercurial/Subversion by encrypting them "at rest" using GnuPG.
* [helm-secrets](https://github.com/jkroepke/helm-secrets) ⭐ 2,023 | 🐛 1 | 🌐 Shell | 📅 2026-08-14 - Helm plugin that helps manage secrets with Git workflow and stores them anywhere, backed by SOPS.
* [Bane](https://github.com/genuinetools/bane) ⭐ 1,230 | 🐛 4 | 🌐 Go | 📅 2020-09-17 - Custom and better AppArmor profile generator for Docker containers.
* [Checkov](https://www.checkov.io/) - Static analysis for Terraform (infrastructure as code) to help detect CIS policy violations and prevent cloud security misconfiguration.
* [Cilium](https://cilium.io/) - Open source software for transparently securing the network connectivity between application services deployed using Linux container management platforms like Docker and Kubernetes.
* [CodeQL](https://securitylab.github.com/tools/codeql) - Discover vulnerabilities across a codebase by performing queries against code as though it were data.
* [DefectDojo](https://www.defectdojo.org/) - Application vulnerability management tool built for DevOps and continuous security integration.
* [Gauntlt](http://gauntlt.org/) - Pentest applications during routine continuous integration build pipelines.
* [Snyk](https://snyk.io/) - Finds and fixes vulnerabilities and license violations in open source dependencies and container images.
* [SonarQube](https://sonarqube.org) - Continuous inspection tool that provides detailed reports during automated testing and alerts on newly introduced security vulnerabilities.
* [Vault](https://www.vaultproject.io/) - Tool for securely accessing secrets such as API keys, passwords, or certificates through a unified interface.
* [git-crypt](https://www.agwa.name/projects/git-crypt/) - Transparent file encryption in git; files which you choose to protect are encrypted when committed, and decrypted when checked out.
* [terrascan](https://runterrascan.io/) - Static code analyzer for Infrastructure as Code tools that helps detect compliance and security violations to mitigate risk before provisioning cloud native resources.
* [tfsec](https://aquasecurity.github.io/tfsec/) - Static analysis security scanner for your Terraform code designed to run locally and in CI pipelines.

### Application or Binary Hardening

* [DynInst](https://dyninst.org/dyninst) - Tools for binary instrumentation, analysis, and modification, useful for binary patching.
* [DynamoRIO](https://dynamorio.org/) - Runtime code manipulation system that supports code transformations on any part of a program, while it executes, implemented as a process-level virtual machine.
* [Egalito](https://egalito.org/) - Binary recompiler and instrumentation framework that can fully disassemble, transform, and regenerate ordinary Linux binaries designed for binary hardening and security research.
* [Valgrind](https://www.valgrind.org/) - Instrumentation framework for building dynamic analysis tools.

### Compliance testing and reporting

* [Chef InSpec](https://www.chef.io/products/chef-inspec) - Language for describing security and compliance rules, which become automated tests that can be run against IT infrastructures to discover and report on non-compliance.
* [OpenSCAP Base](https://www.open-scap.org/tools/openscap-base/) - Both a library and a command line tool (`oscap`) used to evaluate a system against SCAP baseline profiles to report on the security posture of the scanned system(s).

### Dependency confusion

See also [§ Supply chain security](#supply-chain-security).

* [Dependency Combobulator](https://github.com/apiiro/combobulator) ⭐ 95 | 🐛 33 | 🌐 Python | 📅 2024-01-10 - Open source, modular and extensible framework to detect and prevent dependency confusion leakage and potential attacks.
* [Confusion checker](https://github.com/sonatype-nexus-community/repo-diff) ⚠️ Archived - Script to check if you have artifacts containing the same name between your repositories.
* [snync](https://github.com/snyk-labs/snync) ⭐ 53 | 🐛 10 | 🌐 JavaScript | 📅 2026-07-10 - Prevent and detect if you're vulnerable to dependency confusion supply chain security attacks.

### Fuzzing

See also [Awesome-Fuzzing](https://github.com/secfigo/Awesome-Fuzzing) ⭐ 5,894 | 🐛 10 | 📅 2024-04-03.

* [Atheris](https://pypi.org/project/atheris/) - Coverage-guided Python fuzzing engine based off of libFuzzer that supports fuzzing of Python code but also native extensions written for CPython.
* [FuzzBench](https://google.github.io/fuzzbench/) - Free service that evaluates fuzzers on a wide variety of real-world benchmarks, at Google scale.
* [OneFuzz](https://github.com/microsoft/onefuzz) ⚠️ Archived - Self-hosted Fuzzing-as-a-Service (FaaS) platform.

### Policy enforcement

* [AllStar](https://github.com/ossf/allstar) ⭐ 1,441 | 🐛 60 | 🌐 Go | 📅 2026-08-16 - GitHub App installed on organizations or repositories to set and enforce security policies.
* [Tang](https://github.com/latchset/tang) ⭐ 721 | 🐛 41 | 🌐 C | 📅 2025-03-06 - Server for binding data to network presence; provides data to clients only when they are on a certain (secured) network.
* [Conftest](https://conftest.dev/) - Utility to help you write tests against structured configuration data.
* [Open Policy Agent (OPA)](https://www.openpolicyagent.org/) - Unified toolset and framework for policy across the cloud native stack.
* [Regula](https://regula.dev/) - Checks infrastructure as code templates (Terraform, CloudFormation, K8s manifests) for AWS, Azure, Google Cloud, and Kubernetes security and compliance using Open Policy Agent/Rego.

### Supply chain security

See also [§ Dependency confusion](#dependency-confusion).

* [Notary](https://github.com/theupdateframework/notary) ⚠️ Archived - Aims to make the internet more secure by making it easy for people to publish and verify content.
* [Helm GPG (GnuPG) Plugin](https://github.com/technosophos/helm-gpg) ⭐ 29 | 🐛 6 | 🌐 Shell | 📅 2020-02-20 - Chart signing and verification with GnuPG for Helm.
* [Grafeas](https://grafeas.io/) - Open artifact metadata API to audit and govern your software supply chain.
* [in-toto](https://in-toto.io/) - Framework to secure the integrity of software supply chains.

## Honeypots

See also [awesome-honeypots](https://github.com/paralax/awesome-honeypots) ⭐ 10,523 | 🐛 21 | 🌐 Python | 📅 2026-06-01.

* [CanaryTokens](https://github.com/thinkst/canarytokens) ⭐ 2,113 | 🐛 5 | 🌐 Python | 📅 2026-08-13 - Self-hostable honeytoken generator and reporting dashboard; demo version available at [CanaryTokens.org](https://canarytokens.org/).
* [Manuka](https://github.com/spaceraccoon/manuka) ⭐ 348 | 🐛 6 | 🌐 Shell | 📅 2023-05-02 - Open-sources intelligence (OSINT) honeypot that monitors reconnaissance attempts by threat actors and generates actionable intelligence for Blue Teamers.
* [Kushtaka](https://kushtaka.org) - Sustainable all-in-one honeypot and honeytoken orchestrator for under-resourced blue teams.

### Tarpits

* [Endlessh](https://github.com/skeeto/endlessh) ⭐ 8,537 | 🐛 49 | 🌐 C | 📅 2024-06-03 - SSH tarpit that slowly sends an endless banner.
* [LaBrea](http://labrea.sourceforge.net/labrea-info.html) - Program that answers ARP requests for unused IP space, creating the appearance of fake machines that answer further requests very slowly in order to slow down scanners, worms, etcetera.

## Host-based tools

* [Artillery](https://github.com/BinaryDefense/artillery) ⭐ 1,037 | 🐛 25 | 🌐 Python | 📅 2022-01-06 - Combination honeypot, filesystem monitor, and alerting system designed to protect Linux and Windows operating systems.
* [USB Keystroke Injection Protection](https://github.com/google/ukip) ⭐ 548 | 🐛 4 | 🌐 Python | 📅 2023-07-09 - Daemon for blocking USB keystroke injection devices on Linux systems.
* [Crowd Inspect](https://www.crowdstrike.com/resources/community-tools/crowdinspect-tool/) - Free tool for Windows systems aimed to alert you to the presence of malware that may be communicating over the network.
* [Fail2ban](https://www.fail2ban.org/) - Intrusion prevention software framework that protects computer servers from brute-force attacks.
* [Open Source HIDS SECurity (OSSEC)](https://www.ossec.net/) - Fully open source and free, feature-rich, Host-based Instrusion Detection System (HIDS).
* [Rootkit Hunter (rkhunter)](http://rkhunter.sourceforge.net/) - POSIX-compliant Bash script that scans a host for various signs of malware.
* [Shufflecake](https://shufflecake.net/) - Plausible deniability for multiple hidden filesystems on Linux.
* [chkrootkit](http://chkrootkit.org/) - Locally checks for signs of a rootkit on GNU/Linux systems.

### Sandboxes

* [Bubblewrap](https://github.com/containers/bubblewrap) ⭐ 8,382 | 🐛 190 | 🌐 C | 📅 2026-06-02 - Sandboxing tool for use by unprivileged Linux users capable of restricting access to parts of the operating system or user data.
* [Dangerzone](https://dangerzone.rocks/) - Take potentially dangerous PDFs, office documents, or images and convert them to a safe PDF.
* [Firejail](https://firejail.wordpress.com/) - SUID program that reduces the risk of security breaches by restricting the running environment of untrusted applications using Linux namespaces and seccomp-bpf.

## Identity and AuthN/AuthZ

* [Gluu Server](https://gluu.org/) - Central authentication and authorization for Web and mobile applications with a Free and Open Source Software cloud-native community distribution.

## Incident Response tools

See also [awesome-incident-response](https://github.com/meirwah/awesome-incident-response) ⭐ 9,328 | 🐛 73 | 📅 2026-07-15.

* [LogonTracer](https://github.com/JPCERTCC/LogonTracer) ⭐ 3,211 | 🐛 21 | 🌐 Python | 📅 2026-08-02 - Investigate malicious Windows logon by visualizing and analyzing Windows event log.
* [aws\_ir](https://github.com/ThreatResponse/aws_ir) ⭐ 344 | 🐛 14 | 🌐 Python | 📅 2021-07-23 - Automates your incident response with zero security preparedness assumptions.
* [Volatility](https://www.volatilityfoundation.org/) - Advanced memory forensics framework.

### IR management consoles

See also [Security Orchestration, Automation, and Response (SOAR)](#security-orchestration-automation-and-response-soar).

* [Fast Incident Response (FIR)](https://github.com/certsocietegenerale/FIR) ⭐ 2,029 | 🐛 13 | 🌐 JavaScript | 📅 2026-08-07 - Cybersecurity incident management platform allowing for easy creation, tracking, and reporting of cybersecurity incidents.
* [threat\_note](https://github.com/defpoint/threat_note) ⚠️ Archived - Web application built by Defense Point Security to allow security researchers the ability to add and retrieve indicators related to their research.
* [CIRTKit](https://github.com/opensourcesec/CIRTKit) ⭐ 152 | 🐛 0 | 🌐 Python | 📅 2017-04-17 - Scriptable Digital Forensics and Incident Response (DFIR) toolkit built on Viper.
* [Rekall](http://www.rekall-forensic.com/) - Advanced forensic and incident response framework.
* [TheHive](https://thehive-project.org/) - Scalable, free Security Incident Response Platform designed to make life easier for SOCs, CSIRTs, and CERTs, featuring tight integration with MISP.

### Evidence collection

* [OSXAuditor](https://github.com/jipegit/OSXAuditor) ⭐ 3,135 | 🐛 8 | 🌐 JavaScript | 📅 2020-07-27 - Free macOS computer forensics tool.
* [OSXCollector](https://github.com/Yelp/osxcollector) ⚠️ Archived - Forensic evidence collection & analysis toolkit for macOS.
* [Untitled Goose Tool](https://github.com/cisagov/untitledgoosetool) ⭐ 962 | 🐛 17 | 🌐 Python | 📅 2026-02-11 - Assists incident response teams by exporting cloud artifacts from Azure/AzureAD/M365 environments in order to run a full investigation despite lacking in logs ingested by a SIEM.
* [ir-rescue](https://github.com/diogo-fernan/ir-rescue) ⭐ 488 | 🐛 4 | 🌐 Batchfile | 📅 2021-02-21 - Windows Batch script and a Unix Bash script to comprehensively collect host forensic data during incident response.
* [Margarita Shotgun](https://github.com/ThreatResponse/margaritashotgun) ⭐ 253 | 🐛 13 | 🌐 Python | 📅 2020-09-22 - Command line utility (that works with or without Amazon EC2 instances) to parallelize remote memory acquisition.
* [AutoMacTC](https://github.com/CrowdStrike/automactc) - Modular, automated forensic triage collection framework designed to access various forensic artifacts on macOS, parse them, and present them in formats viable for analysis.

## Network perimeter defenses

* [ssh-audit](https://github.com/jtesta/ssh-audit) ⭐ 4,259 | 🐛 38 | 🌐 Python | 📅 2026-07-09 - Simple tool that makes quick recommendations for improving an SSH server's security posture.
* [Gatekeeper](https://github.com/AltraMayor/gatekeeper) ⭐ 1,630 | 🐛 96 | 🌐 C | 📅 2025-11-05 - First open source Distributed Denial of Service (DDoS) protection system.
* [fwknop](https://www.cipherdyne.org/fwknop/) - Protects ports via Single Packet Authorization in your firewall.

### Firewall appliances or distributions

See also [Wikipedia: List of router and firewall distributions](https://en.wikipedia.org/wiki/List_of_router_and_firewall_distributions).

* [IPFire](https://www.ipfire.org/) - Hardened GNU/Linux based router and firewall distribution forked from IPCop.
* [OPNsense](https://opnsense.org/) - Hardened FreeBSD based firewall and routing platform forked from pfSense.
* [pfSense](https://www.pfsense.org/) - FreeBSD firewall and router distribution forked from m0n0wall.

## Operating System distributions

* [Computer Aided Investigative Environment (CAINE)](https://caine-live.net/) - Italian GNU/Linux live distribution that pre-packages numerous digital forensics and evidence collection tools.
* [Security Onion](https://securityonionsolutions.com/) - Free and open source GNU/Linux distribution for intrusion detection, enterprise security monitoring, and log management.
* [Qubes OS](https://qubes-os.org/) - Desktop environment built atop the Xen hypervisor project that runs each end-user program in its own virtual machine intended to provide strict security controls to constrain the reach of any successful malware exploit.

## Phishing awareness and reporting

See also [awesome-pentest § Social Engineering Tools](https://github.com/fabacab/awesome-pentest#social-engineering-tools) ⭐ 280 | 🐛 0 | 📅 2023-10-23.

* [King Phisher](https://github.com/securestate/king-phisher) ⭐ 2,575 | 🐛 2 | 🌐 Python | 📅 2026-08-04 - Tool for testing and promoting user awareness by simulating real world phishing attacks.
* [phishing\_catcher](https://github.com/x0rz/phishing_catcher) ⭐ 1,817 | 🐛 44 | 🌐 Python | 📅 2024-08-13 - Configurable script to watch for issuances of suspicious TLS certificates by domain name in the Certificate Transparency Log (CTL) using the [CertStream](https://certstream.calidog.io/) service.
* [CertSpotter](https://github.com/SSLMate/certspotter) ⭐ 1,164 | 🐛 20 | 🌐 Go | 📅 2026-07-29 - Certificate Transparency log monitor from SSLMate that alerts you when a SSL/TLS certificate is issued for one of your domains.
* [Swordphish](https://github.com/certsocietegenerale/swordphish-awareness) ⭐ 226 | 🐛 6 | 🌐 Python | 📅 2024-09-22 - Platform allowing to create and manage (fake) phishing campaigns intended to train people in identifying suspicious mails.
* [Phishing Intelligence Engine (PIE)](https://github.com/LogRhythm-Labs/PIE) ⭐ 179 | 🐛 8 | 🌐 PowerShell | 📅 2020-04-13 - Framework that will assist with the detection and response to phishing attacks.
* [mailspoof](https://github.com/serain/mailspoof) ⭐ 138 | 🐛 13 | 🌐 Python | 📅 2022-12-08 - Scans SPF and DMARC records for issues that could allow email spoofing.
* [NotifySecurity](https://github.com/certsocietegenerale/NotifySecurity) ⚠️ Archived - Outlook add-in used to help your users to report suspicious e-mails to security teams.
* [Gophish](https://getgophish.com/) - Powerful, open-source phishing framework that makes it easy to test your organization's exposure to phishing.

## Preparedness training and wargaming

(Also known as *adversary emulation*, *threat simulation*, or similar.)

* [APTSimulator](https://github.com/NextronSystems/APTSimulator) ⭐ 2,761 | 🐛 4 | 🌐 Batchfile | 📅 2025-09-23 - Toolset to make a system look as if it was the victim of an APT attack.
* [Network Flight Simulator (`flightsim`)](https://github.com/alphasoc/flightsim) ⭐ 1,362 | 🐛 25 | 🌐 Go | 📅 2024-04-04 - Utility to generate malicious network traffic and help security teams evaluate security controls and audit their network visibility.
* [RedHunt OS](https://github.com/redhuntlabs/RedHunt-OS) ⭐ 1,317 | 🐛 7 | 📅 2025-01-22 - Ubuntu-based Open Virtual Appliance (`.ova`) preconfigured with several threat emulation tools as well as a defender's toolkit.
* [Metta](https://github.com/uber-common/metta) ⭐ 1,145 | 🐛 13 | 🌐 Python | 📅 2019-04-01 - Automated information security preparedness tool to do adversarial simulation.
* [DumpsterFire](https://github.com/TryCatchHCF/DumpsterFire) ⭐ 1,039 | 🐛 4 | 🌐 Python | 📅 2020-05-27 - Modular, menu-driven, cross-platform tool for building repeatable, time-delayed, distributed security events for Blue Team drills and sensor/alert mapping.
* [Atomic Red Team](https://atomicredteam.io/) - Library of simple, automatable tests to execute for testing security controls.
* [BadBlood](https://www.secframe.com/badblood/) - Fills a test (non-production) Windows Domain with data that enables security analysts and engineers to practice using tools to gain an understanding and prescribe to securing Active Directory.
* [Caldera](https://caldera.mitre.org/) - Scalable, automated, and extensible adversary emulation platform developed by MITRE.
* [Drool](https://www.dns-oarc.net/tools/drool) - Replay DNS traffic from packet capture files and send it to a specified server, such as for simulating DDoS attacks on the DNS and measuring normal DNS querying.
* [Infection Monkey](https://www.guardicore.com/infectionmonkey/) - Open-source breach and attack simulation (BAS) platform that helps you validate existing controls and identify how attackers might exploit your current network security gaps.
* [Stratus Red Team](https://stratus-red-team.cloud/) - Emulate offensive attack techniques in a granular and self-contained manner against a cloud environment; think "Atomic Red Team™ for the cloud."
* [tcpreplay](https://tcpreplay.appneta.com/) - Suite of free Open Source utilities for editing and replaying previously captured network traffic originally designed to replay malicious traffic patterns to Intrusion Detection/Prevention Systems.

### Post-engagement analysis and reporting

* [RedEye](https://cisagov.github.io/RedEye/) - Analytic tool to assist both Red and Blue teams with visualizing and reporting command and control activities, replay and demonstrate attack paths, and more clearly communicate remediation recommendations to stakeholders.

## Security configurations

(Also known as *secure-by-default baselines* and *implemented best practices*.)

* [Bunkerized-nginx](https://github.com/bunkerity/bunkerized-nginx) ⭐ 10,810 | 🐛 179 | 🌐 Python | 📅 2026-08-14 - Docker image of an NginX configuration and scripts implementing many defensive techniques for Web sites.

## Security monitoring

* [Crossfeed](https://docs.crossfeed.cyber.dhs.gov/) - Continuously enumerates and monitors an organization’s public-facing attack surface in order to discover assets and flag potential security flaws.
* [Starbase](https://github.com/JupiterOne/starbase) ⭐ 362 | 🐛 15 | 🌐 TypeScript | 📅 2026-02-19 - Collects assets and relationships from services and systems into an intuitive graph view to offer graph-based security analysis for everyone.

### Endpoint Detection and Response (EDR)

* [Wazuh](https://wazuh.com/) - Open source, multiplatform agent-based security monitoring based on a fork of OSSEC HIDS.

### Network Security Monitoring (NSM)

See also [awesome-pcaptools](https://github.com/caesar0301/awesome-pcaptools) ⭐ 3,413 | 🐛 14 | 📅 2025-09-03.

* [Tsunami](https://github.com/google/tsunami-security-scanner) ⭐ 8,604 | 🐛 13 | 🌐 Java | 📅 2026-06-23 - General purpose network security scanner with an extensible plugin system for detecting high severity vulnerabilities with high confidence.
* [Maltrail](https://github.com/stamparm/maltrail) ⭐ 8,581 | 🐛 89 | 🌐 Rust | 📅 2026-08-16 - Malicious network traffic detection system.
* [Arkime](https://github.com/arkime/arkime) ⭐ 7,447 | 🐛 36 | 🌐 C | 📅 2026-08-16 - Augments your current security infrastructure to store and index network traffic in standard PCAP format, providing fast, indexed access.
* [Stenographer](https://github.com/google/stenographer) ⚠️ Archived - Full-packet-capture utility for buffering packets to disk for intrusion detection and incident response purposes.
* [VAST](https://github.com/tenzir/vast) ⭐ 754 | 🐛 0 | 🌐 C++ | 📅 2026-08-14 - Free and open-source network telemetry engine for data-driven security investigations.
* [Real Intelligence Threat Analysis (RITA)](https://github.com/activecm/rita) ⭐ 622 | 🐛 25 | 🌐 Go | 📅 2026-06-17 - Open source framework for network traffic analysis that ingests Zeek logs and detects beaconing, DNS tunneling, and more.
* [ChopShop](https://github.com/MITRECND/chopshop) ⚠️ Archived - Framework to aid analysts in the creation and execution of pynids-based decoders and detectors of APT tradecraft.
* [Respounder](https://github.com/codeexpress/respounder) ⭐ 323 | 🐛 1 | 🌐 Go | 📅 2019-06-15 - Detects the presence of the Responder LLMNR/NBT-NS/MDNS poisoner on a network.
* [SpoofSpotter](https://github.com/NetSPI/SpoofSpotter) ⭐ 51 | 🐛 1 | 🌐 Python | 📅 2018-06-13 - Catch spoofed NetBIOS Name Service (NBNS) responses and alert to an email or log file.
* [OwlH](https://www.owlh.net/) - Helps manage network IDS at scale by visualizing Suricata, Zeek, and Moloch life cycles.
* [Snort](https://snort.org/) - Widely-deployed, Free Software IPS capable of real-time packet analysis, traffic logging, and custom rule-based triggers.
* [Suricata](https://suricata-ids.org/) - Free, cross-platform, IDS/IPS with on- and off-line analysis modes and deep packet inspection capabilities that is also scriptable with Lua.
* [Wireshark](https://www.wireshark.org) - Free and open-source packet analyzer useful for network troubleshooting or forensic netflow analysis.
* [Zeek](https://zeek.org/) - Powerful network analysis framework focused on security monitoring, formerly known as Bro.
* [netsniff-ng](http://netsniff-ng.org/) -  Free and fast GNU/Linux networking toolkit with numerous utilities such as a connection tracking tool (`flowtop`), traffic generator (`trafgen`), and autonomous system (AS) trace route utility (`astraceroute`).

### Security Information and Event Management (SIEM)

* [AlienVault OSSIM](https://www.alienvault.com/open-threat-exchange/projects) - Single-server open source SIEM platform featuring asset discovery, asset inventorying, behavioral monitoring, and event correlation, driven by AlienVault Open Threat Exchange (OTX).
* [Prelude SIEM OSS](https://www.prelude-siem.org/) - Open source, agentless SIEM with a long history and several commercial variants featuring security event collection, normalization, and alerting from arbitrary log input and numerous popular monitoring tools.

### Service and performance monitoring

See also [awesome-sysadmin#monitoring](https://github.com/n1trux/awesome-sysadmin#monitoring) ⭐ 34,912 | 🐛 0 | 📅 2026-08-16.

* [Icinga](https://icinga.com/) - Modular redesign of Nagios with pluggable user interfaces and an expanded set of data connectors, collectors, and reporting tools.
* [Locust](https://locust.io/) - Open source load testing tool in which you can define user behaviour with Python code and swarm your system with millions of simultaneous users.
* [Nagios](https://nagios.org) - Popular network and service monitoring solution and reporting platform.
* [OpenNMS](https://opennms.org/) - Free and feature-rich networking monitoring system supporting multiple configurations, a variety of alerting mechanisms (email, XMPP, SMS), and numerous data collection methods (SNMP, HTTP, JDBC, etc).
* [osquery](https://github.com/facebook/osquery) ⭐ 23,468 | 🐛 618 | 🌐 C++ | 📅 2026-08-13 - Operating system instrumentation framework for macOS, Windows, and Linux, exposing the OS as a high-performance relational database that can be queried with a SQL-like syntax.
* [Zabbix](https://www.zabbix.com/) - Mature, enterprise-level platform to monitor large-scale IT environments.

### Threat hunting

(Also known as *hunt teaming* and *threat detection*.)

See also [awesome-threat-detection](https://github.com/0x4D31/awesome-threat-detection) ⭐ 4,700 | 🐛 54 | 📅 2026-01-05.

* [GRR Rapid Response](https://github.com/google/grr) ⭐ 5,088 | 🐛 191 | 🌐 Python | 📅 2026-05-12 - Incident response framework focused on remote live forensics consisting of a Python agent installed on assets and Python-based server infrastructure enabling analysts to quickly triage attacks and perform analysis remotely.
* [Hunting ELK (HELK)](https://github.com/Cyb3rWard0g/HELK) ⭐ 3,929 | 🐛 60 | 🌐 Jupyter Notebook | 📅 2024-06-01 - All-in-one Free Software threat hunting stack based on Elasticsearch, Logstash, Kafka, and Kibana with various built-in integrations for analytics including Jupyter Notebook.
* [DeepBlueCLI](https://github.com/sans-blue-team/DeepBlueCLI) ⭐ 2,427 | 🐛 13 | 🌐 PowerShell | 📅 2023-10-14 - PowerShell module for hunt teaming via Windows Event logs.
* [MozDef](https://github.com/mozilla/MozDef) ⚠️ Archived - Automate the security incident handling process and facilitate the real-time activities of incident handlers.
* [PowerForensics](https://github.com/Invoke-IR/PowerForensics) ⭐ 1,442 | 🐛 64 | 🌐 C# | 📅 2023-11-16 - All in one PowerShell-based platform to perform live hard disk forensic analysis.
* [CimSweep](https://github.com/PowerShellMafia/CimSweep) ⭐ 656 | 🐛 2 | 🌐 PowerShell | 📅 2019-08-19 - Suite of CIM/WMI-based tools enabling remote incident response and hunting operations across all versions of Windows.
* [PSRecon](https://github.com/gfoss/PSRecon) ⭐ 494 | 🐛 4 | 🌐 PowerShell | 📅 2017-07-29 - PSHunt-like tool for analyzing remote Windows systems that also produces a self-contained HTML report of its findings.
* [PSHunt](https://github.com/Infocyte/PSHunt) ⚠️ Archived - PowerShell module designed to scan remote endpoints for indicators of compromise or survey them for more comprehensive information related to state of those systems.
* [rastrea2r](https://github.com/rastrea2r/rastrea2r) ⭐ 238 | 🐛 8 | 🌐 Python | 📅 2021-08-01 - Multi-platform tool for triaging suspected IOCs on many endpoints simultaneously and that integrates with antivirus consoles.
* [Logging Made Easy (LME)](https://www.cisa.gov/resources-tools/services/logging-made-easy) - Free and open logging and protective monitoring solution serving.
* [Redline](https://www.fireeye.com/services/freeware/redline.html) - Freeware endpoint auditing and analysis tool that provides host-based investigative capabilities, offered by FireEye, Inc.

## Threat intelligence

See also [awesome-threat-intelligence](https://github.com/hslatman/awesome-threat-intelligence) ⭐ 10,538 | 🐛 116 | 📅 2026-05-31.

* [Sigma](https://github.com/Neo23x0/sigma) ⭐ 10,890 | 🐛 199 | 🌐 Python | 📅 2026-08-15 - Generic signature format for SIEM systems, offering an open signature format that allows you to describe relevant log events in a straightforward manner.
* [YARA](https://github.com/VirusTotal/yara) ⭐ 9,812 | 🐛 177 | 🌐 C | 📅 2026-07-30 - Tool aimed at (but not limited to) helping malware researchers to identify and classify malware samples, described as "the pattern matching swiss army knife" for file patterns and signatures.
* [Viper](https://github.com/viper-framework/viper) ⚠️ Archived - Binary analysis and management framework enabling easy organization of malware and exploit samples.
* [GRASSMARLIN](https://github.com/nsacyber/GRASSMARLIN) ⚠️ Archived - Provides IP network situational awareness of industrial control systems (ICS) and Supervisory Control and Data Acquisition (SCADA) by passively mapping, accounting for, and reporting on your ICS/SCADA network topology and endpoints.
* [ThreatIngestor](https://github.com/InQuest/ThreatIngestor) ⭐ 922 | 🐛 15 | 🌐 Python | 📅 2026-05-26 - Extendable tool to extract and aggregate IOCs from threat feeds including Twitter, RSS feeds, or other sources.
* [MLSec Combine](https://github.com/mlsecproject/combine) ⭐ 656 | 🐛 45 | 🌐 Python | 📅 2019-03-14 - Gather and combine multiple threat intelligence feed sources into one customizable, standardized CSV-based format.
* [Threat Bus](https://github.com/tenzir/threatbus) ⚠️ Archived - Threat intelligence dissemination layer to connect security tools through a distributed publish/subscribe message broker.
* [Forager](https://github.com/opensourcesec/Forager) ⭐ 178 | 🐛 3 | 🌐 Python | 📅 2018-01-23 - Multi-threaded threat intelligence gathering built with Python3 featuring simple text-based configuration and data storage for ease of use and data portability.
* [DATA](https://github.com/hadojae/DATA) ⭐ 99 | 🐛 15 | 🌐 Python | 📅 2018-08-22 - Credential phish analysis and automation tool that can accept suspected phishing URLs directly or trigger on observed network traffic containing such a URL.
* [AttackerKB](https://attackerkb.com/) - Free and public crowdsourced vulnerability assessment platform to help prioritize high-risk patch application and combat vulnerability fatigue.
* [Malware Information Sharing Platform and Threat Sharing (MISP)](https://misp-project.org/) - Open source software solution for collecting, storing, distributing and sharing cyber security indicators.
* [Open Source Vulnerabilities (OSV)](https://osv.dev/) - Vulnerability database and triage infrastructure for open source projects aimed at helping both open source maintainers and consumers of open source.
* [Unfetter](https://nsacyber.github.io/unfetter/) - Identifies defensive gaps in security posture by leveraging Mitre's ATT\&CK framework.

### Fingerprinting

* [HASSH](https://github.com/salesforce/hassh) ⚠️ Archived - Network fingerprinting standard which can be used to identify specific client and server SSH implementations.
* [JA3](https://ja3er.com/) - Extracts SSL/TLS handshake settings for fingerprinting and communicating about a given TLS implementation.

### Threat signature packages and collections

* [YARA Rules](https://github.com/Yara-Rules/rules) ⭐ 4,874 | 🐛 28 | 🌐 YARA | 📅 2024-04-17 - Project covering the need for IT security researchers to have a single repository where different Yara signatures are compiled, classified and kept as up to date as possible.
* [FireEye's Red Team Tool Countermeasures](https://github.com/fireeye/red_team_tool_countermeasures) ⚠️ Archived - Collection of Snort and YARA rules to detect attacks carried out with FireEye's own Red Team tools, first released after FireEye disclosed a breach in December 2020.
* [ESET's Malware IoCs](https://github.com/eset/malware-ioc) ⭐ 1,976 | 🐛 0 | 🌐 YARA | 📅 2026-06-25 - Indicators of Compromises (IOCs) derived from ESET's various investigations.
* [FireEye's Sunburst Countermeasures](https://github.com/fireeye/sunburst_countermeasures) ⚠️ Archived - Collection of IoC in various languages for detecting backdoored SolarWinds Orion NMS activities and related vulnerabilities.

## Tor Onion service defenses

See also [awesome-tor](https://github.com/ajvb/awesome-tor) ⭐ 504 | 🐛 3 | 📅 2023-09-03.

* [OnionBalance](https://onionbalance.readthedocs.io/) - Provides load-balancing while also making Onion services more resilient and reliable by eliminating single points-of-failure.
* [Vanguards](https://github.com/mikeperry-tor/vanguards) ⭐ 246 | 🐛 30 | 🌐 Python | 📅 2024-07-06 - Version 3 Onion service guard discovery attack mitigation script (intended for eventual inclusion in Tor core).

## Transport-layer defenses

* [Certbot](https://certbot.eff.org/) - Free tool to automate the issuance and renewal of TLS certificates from the [LetsEncrypt Root CA](https://letsencrypt.org/) with plugins that configure various Web and e-mail server software.
* [MITMEngine](https://github.com/cloudflare/mitmengine) ⚠️ Archived - Golang library for server-side detection of TLS interception events.
* [Tor](https://torproject.org/) - Censorship circumvention and anonymizing overlay network providing distributed, cryptographically verified name services (`.onion` domains) to enhance publisher privacy and service availability.

### Overlay and Virtual Private Networks (VPNs)

* [Headscale](https://github.com/juanfont/headscale) ⭐ 42,899 | 🐛 142 | 🌐 Go | 📅 2026-07-30 - Open source, self-hosted implementation of the Tailscale control server.
* [IPsec VPN Server Auto Setup Scripts](https://github.com/hwdsl2/setup-ipsec-vpn) ⭐ 28,344 | 🐛 1 | 🌐 Shell | 📅 2026-08-15 - Scripts to build your own IPsec VPN server, with IPsec/L2TP, Cisco IPsec and IKEv2.
* [Nebula](https://github.com/slackhq/nebula) ⭐ 17,619 | 🐛 102 | 🌐 Go | 📅 2026-08-14 - Completely open source and self-hosted, scalable overlay networking tool with a focus on performance, simplicity, and security, inspired by tinc.
* [Innernet](https://github.com/tonarino/innernet) ⭐ 5,523 | 🐛 83 | 🌐 Rust | 📅 2026-07-28 - Free Software private network system that uses WireGuard under the hood, made to be self-hosted.
* [Firezone](https://www.firezone.dev/) - Self-hosted VPN server built on WireGuard that supports MFA and SSO.
* [OpenVPN](https://openvpn.net/) - Longstanding Free Software traditional SSL/TLS-based virtual private network.
* [OpenZITI](https://openziti.github.io/) - Open source initiative focused on bringing Zero Trust to any application via an overlay network, tunelling applications, and numerous SDKs.
* [Tailscale](https://tailscale.com/) - Managed freemium mesh VPN service built on top of WireGuard.
* [WireGuard](https://www.wireguard.com/) - Extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography.
* [tinc](https://tinc-vpn.org/) - Free Software mesh VPN implemented entirely in userspace that supports expandable network space, bridged ethernet segments, and more.

## macOS-based defenses

See also [drduh/macOS-Security-and-Privacy-Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide) ⭐ 22,495 | 🐛 8 | 📅 2026-08-10.

* [Santa](https://github.com/google/santa) ⚠️ Archived - Keep track of binaries that are naughty or nice in an allow/deny-listing system for macOS.
* [Stronghold](https://github.com/alichtman/stronghold) ⭐ 1,191 | 🐛 10 | 🌐 Python | 📅 2025-02-24 - Easily configure macOS security settings from the terminal.
* [macOS Fortress](https://github.com/essandess/macOS-Fortress) ⭐ 451 | 🐛 1 | 🌐 Shell | 📅 2021-11-24 - Automated configuration of kernel-level, OS-level, and client-level security features including privatizing proxying and anti-virus scanning for macOS.
* [BlockBlock](https://objective-see.com/products/blockblock.html) - Monitors common persistence locations and alerts whenever a persistent component is added, which helps to detect and prevent malware installation.
* [LuLu](https://objective-see.com/products/lulu.html) - Free macOS firewall.

## Windows-based defenses

See also [awesome-windows#security](https://github.com/Awesome-Windows/Awesome#security) and [awesome-windows-domain-hardening](https://github.com/PaulSec/awesome-windows-domain-hardening) ⭐ 1,796 | 🐛 1 | 📅 2020-01-07.

* [HardenTools](https://github.com/securitywithoutborders/hardentools) ⭐ 3,105 | 🐛 12 | 🌐 Go | 📅 2025-08-10 - Utility that disables a number of risky Windows features.
* [Windows Secure Host Baseline](https://github.com/nsacyber/Windows-Secure-Host-Baseline) ⚠️ Archived - Group Policy objects, compliance checks, and configuration tools that provide an automated and flexible approach for securely deploying and maintaining the latest releases of Windows 10.
* [CobaltStrikeScan](https://github.com/Apr4h/CobaltStrikeScan) ⭐ 919 | 🐛 3 | 🌐 C# | 📅 2021-08-19 - Scan files or process memory for Cobalt Strike beacons and parse their configuration.
* [Sticky Keys Slayer](https://github.com/linuz/Sticky-Keys-Slayer) ⭐ 347 | 🐛 15 | 🌐 Shell | 📅 2018-03-16 - Establishes a Windows RDP session from a list of hostnames and scans for accessibility tools backdoors, alerting if one is discovered.
* [WMI Monitor](https://github.com/realparisi/WMI_Monitor) ⭐ 123 | 🐛 2 | 🌐 PowerShell | 📅 2018-02-28 - Log newly created WMI consumers and processes to the Windows Application event log.
* [NotRuler](https://github.com/sensepost/notruler) ⭐ 96 | 🐛 3 | 🌐 Go | 📅 2017-10-11 - Detect both client-side rules and VBScript enabled forms used by the [Ruler](https://github.com/sensepost/ruler) ⭐ 2,314 | 🐛 14 | 🌐 Go | 📅 2024-06-10 attack tool when attempting to compromise a Microsoft Exchange server.
* [Sandboxie](https://www.sandboxie.com/) - Free and open source general purpose Windows application sandboxing utility.
* [Sigcheck](https://docs.microsoft.com/en-us/sysinternals/downloads/sigcheck) - Audit a Windows host's root certificate store against Microsoft's [Certificate Trust List (CTL)](https://docs.microsoft.com/en-us/windows/desktop/SecCrypto/certificate-trust-list-overview).

### Active Directory

* [PlumHound](https://github.com/PlumHound/PlumHound) ⭐ 1,309 | 🐛 7 | 🌐 Python | 📅 2025-11-15 - More effectively use BloodHoundAD in continual security life-cycles by utilizing its pathfinding engine to identify Active Directory security vulnerabilities.
* [Active Directory Control Paths](https://github.com/ANSSI-FR/AD-control-paths) ⚠️ Archived - Visualize and graph Active Directory permission configs ("control relations") to audit questions such as "Who can read the CEO's email?" and similar.
* [PingCastle](https://www.pingcastle.com/) - Active Directory vulnerability detection and reporting tool.

## License

[![CC-BY](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by.svg)](https://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-16._
