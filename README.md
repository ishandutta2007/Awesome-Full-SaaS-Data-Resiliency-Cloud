# Awesome-Full-SaaS-Data-Resiliency-Cloud

## Top 100% SaaS Data Resiliency Cloud Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Cloud-Native Backup, Ransomware Recovery & Self-Hosted Data Protection Engines*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **100% SaaS Data Resiliency Clouds**. These offerings provide fully managed, cloud-native data protection—covering everything from backup for SaaS applications like Microsoft 365 and Salesforce to cyber recovery and ransomware resilience, with no on-premises infrastructure required. The category spans **pure SaaS platforms** with consumption-based pricing and **open-source engines** that bring cloud-native data protection principles to self-hosted deployments.

**Examples** include Druva Data Resiliency Cloud, Rubrik Security Cloud, Cohesity Cloud Services, Commvault Cloud (Metallic), Veeam Data Cloud, Clumio, Keepit, and Plakar (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted data resiliency, open-source backup engines with end-to-end encryption, and community-driven recovery validation—ideal for organizations seeking data sovereignty and avoiding per-TB consumption fees that compound as data estates grow. The open-source landscape is genuinely emerging: **Plakar** offers an open resilience standard with audited end-to-end encryption and deduplication , while **Backrest** provides a web UI and orchestrator for Restic backups .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva Data Resiliency Cloud](https://www.druva.com/)** | **The purest 100% SaaS data protection platform.** Cloud-native backup for SaaS apps, endpoints, data centers, and cloud workloads with **global deduplication and zero-egress restores**. **Credit-based consumption**: 1 credit = 1 TB of compressed/deduplicated data stored for one month, tracked daily. Plans: **Business** (core protection), **Enterprise** (adds cross-cloud backup and automated DR), **Elite** (fullest feature set) . | **Per TB/month after deduplication**; Business/Enterprise/Elite tiers quote-only . Example: 90 TB source dedupes 3:1 to ~30 credits/month . | No free tier; trial via sales |
| **[Rubrik Security Cloud](https://www.rubrik.com/)** | Cyber resilience platform with immutable backups, threat monitoring, and orchestrated recovery. **Scale Subscription** (3-year minimum, extendable to 5) with **BETB measurement on-prem and FETB for cloud**. **Utility** model for variable workloads (reserve capacity + on-demand). **Rubrik Cloud Vault** for hosted backup storage . | **Foundation: $156K/year** (100 BETB list); Business: **$195.6K**; Enterprise: **$273.6K** . 3-year minimum common . | No free tier; trial via sales |
| **[Cohesity Cloud Services](https://www.cohesity.com/)** | Fully managed multicloud BaaS hosted in AWS/Azure/GCP. **Cohesity Cloud for M365** available on AWS and Azure data planes with Core and Unlimited editions. Eliminates CapEx with subscription pricing . | **M365 Cloud Protection** via SHI: Core (80 FETB, 1 user) **~$69/month**; Unlimited (1 user) **~$34–$50/month** depending on region/tier . Enterprise BaaS: quote-only. | No free tier; trial via sales |
| **[Commvault Cloud (Metallic)](https://www.commvault.com/)** | SaaS-delivered data protection with **Metallic Cloud Storage Service** as a fully managed backup target. Integrated with Commvault Backup & Recovery; leverages Microsoft Azure technology . | **Metallic Cloud Storage**: Cool Tier **~$937–$1,020/TB/month**; Hot Tier **~$2,340/TB/month** (1-month subscription) . | No free tier; trial via sales |
| **[Veeam Data Cloud](https://www.veeam.com/)** | Fully managed SaaS backup with **unlimited storage included**. **Foundation ($2.63/user/mo annual)**: M365 backup (Exchange, SharePoint, OneDrive, Teams). **Advanced ($3.33)**: adds Entra ID resilience. **Premium ($7.00)**: adds disaster recovery with no throttling. **Veeam Vault** add-on for immutable cloud storage: Archive **$14/TB/mo**, Standard **$24/TB/mo** . | **M365 Foundation: $2.63/user/month** (annual, 251+ users); Advanced: **$3.33**; Premium: **$7.00** . Vault: **$14–$24/TB/month** . | No free tier; trial available |
| **[Clumio (by Commvault)](https://www.commvault.com/)** | Fully managed, air-gapped cloud backup for AWS and Microsoft 365. **API-first with Terraform provider**. **SecureVault** offering for S3-compatible storage with air gap and cross-region restore . | **S3 backup: $0.025/GiB-month** + $1.50/million managed objects; Aurora: **$0.030/GiB-mo**; DynamoDB: **$0.15/GiB-mo** + $0.02/million items; GCS: **$0.027/GiB-mo** . Restore fees apply. | No free tier; trial available |
| **[Keepit](https://www.keepit.com/)** | Independent cloud backup for SaaS apps (Microsoft 365, Google Workspace, Salesforce, Dynamics 365). **Vendor-independent data centers**, immutable blockchain-verified storage, 4 copies in 2 data centers per region. **No egress, ingress, or transaction fees** . | Quote-only (per-user or per-data-volume) | No free tier; trial available |
| **[HYCU Protégé](https://www.hycu.com/)** | Multi-cloud data protection with **Nutanix heritage**. 100+ workloads across AWS, Azure, GCP, and SaaS apps. Agentless, WORM-backed, ransomware readiness architecture. | Quote-only (usage-based per VM/TiB/GiB) | Free trial available |
| **[Acronis Cyber Cloud](https://www.acronis.com/)** | Cyber protection platform combining backup, disaster recovery, and AI-based ransomware detection. Service provider-focused with per-workload or per-GB pricing. | Quote-only (per-workload or per-GB) | Free licensing model for service provider onboarding |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Plakar](https://github.com/plakarkorp/plakar)** | [![Stars](https://img.shields.io/github/stars/plakarkorp/plakar?style=social&color=white)](https://github.com/plakarkorp/plakar/stargazers) | **The most ambitious open-source "resilience standard" with audited end-to-end encryption.** **ISC licensed core—free forever** for agent installation, single-store management, backup/navigation/restore via CLI, with **source-side encryption and deduplication** . **Kloset format**: deduplicated, compressed, **end-to-end encrypted, verifiable** data container that can move to NAS, S3, tape, or databases while retaining granular restore capability . **Zero-trust architecture**: encryption keys derived from passphrase never stored; audited by independent expert with public reports . **Enterprise edition** adds multi-store orchestration, RBAC, KMS/Vault integration, and compliance audits . **Best for organizations wanting a modern, auditable open-source backup engine** with cryptographic guarantees. |
| **[Backrest](https://github.com/garethgeorge/backrest)** | [![Stars](https://img.shields.io/github/stars/garethgeorge/backrest?style=social&color=white)](https://github.com/garethgeorge/backrest/stargazers) | **Web UI and orchestrator for restic backup repositories.** **Self-hosted** with a clean interface for managing multiple restic repos, scheduling backup plans, browsing snapshots, and restoring files—bringing a Veeam-like management experience to the restic ecosystem . **Best for teams already using restic** wanting a centralized management layer without SaaS fees. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Restic](https://github.com/restic/restic)** | [![Stars](https://img.shields.io/github/stars/restic/restic?style=social&color=white)](https://github.com/restic/restic/stargazers) | **The foundational open-source backup engine that powers Backrest and many self-hosted SaaS-like workflows.** Encrypted, deduplicated, supports S3/B2/Azure/GCS/SFTP. **No central management**—pair with Backrest or custom tooling . **Best as the storage engine** beneath a self-hosted resiliency stack . |
| **[Kopia](https://github.com/kopia/kopia)** | [![Stars](https://img.shields.io/github/stars/kopia/kopia?style=social&color=white)](https://github.com/kopia/kopia/stargazers) | **Cross-platform backup with GUI and repository server.** Same deduplicated, encrypted chunk-based design as Restic but adds a **desktop app and optional repository server** for centralized management. **Best for mixed-OS environments** where CLI-only tools are impractical . |

**Frameworks for building custom systems**: Choose **Plakar** for an audited open-source backup engine with end-to-end encryption and verifiable Klosets , **Backrest** for a web-managed restic orchestration layer , or **Kopia** for cross-platform backup with a built-in server —all without per-TB consumption fees that compound as data estates grow.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- SaaS data resiliency platforms handle critical business data; enforce encryption at rest and in transit, strong access controls, and regular restore testing. **A backup that cannot be restored is not a backup.**
- **Pricing models in this category are consumption-based and can compound unpredictably.** **Druva's credit model** tracks deduplicated data stored daily—change rate, retention, and dedupe efficiency all move the bill . **Rubrik's 3-year minimum** with **BETB/FETB measurement** means cloud customers pay on raw data volume regardless of deduplication effectiveness . **Veeam Data Cloud's unlimited storage** is genuinely included in per-user pricing ($2.63–$7.00/user/mo) , but **Vault add-on storage costs $14–$24/TB/month** . **Clumio's per-GiB pricing** ($0.025–$0.15/GiB-mo depending on workload) plus restore fees requires careful volume modeling . **Plakar's open-source core is ISC-licensed and free forever** with audited encryption—the trade-off is self-hosting and operational responsibility . **Validate whether you need a fully managed SaaS platform (Druva, Rubrik, Veeam) or a self-hosted open-source engine (Plakar, Backrest)** before committing.

---

**Made for data protection architects, SREs, and organizations building cloud-native resilience.**  
Let's make SaaS data resiliency more open, auditable, and cost-predictable.
