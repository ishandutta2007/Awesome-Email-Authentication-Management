# Awesome-Email-Authentication-Management

## Top Email Authentication Management Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on DMARC Enforcement, SPF/DKIM Alignment, BIMI Deployment & Email Fraud Defense*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Email Authentication Management**. These tools help organizations monitor DMARC aggregate reports, troubleshoot SPF and DKIM alignment failures, enforce p=quarantine/p=reject policies, and deploy BIMI for brand trust.

**Examples** include Valimail, EasyDMARC, dmarcian, PowerDMARC, Red Sift OnDMARC, Mimecast DMARC Analyzer, Proofpoint Email Fraud Defense, Sendmarc, URIports, and DMARCLY (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom report parsing, and transparent email authentication data — ideal for MSPs and security teams that want unlimited domain monitoring without per-report SaaS quotas or vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Valimail](https://www.valimail.com/)**
  DMARC and email authentication platform with automated enforcement. Provides continuous monitoring, sender identification, and BIMI deployment for enterprises.

- **[EasyDMARC](https://easydmarc.com/)**
  DMARC management platform with affordable pricing for SMBs and MSPs. Provides aggregate report parsing, SPF flattening, and hosted DMARC records.

- **[dmarcian](https://dmarcian.com/)**
  Veteran DMARC platform known for its education-focused approach and free tier. Provides report analysis, sender identification, and phased enforcement guidance.

- **[PowerDMARC](https://powerdmarc.com/)**
  Multi-tenant DMARC, SPF, DKIM, and BIMI management platform. Strong MSP features with white-labeling and API access.

- **[Red Sift OnDMARC](https://redsift.com/)**
  Enterprise DMARC platform with advanced analytics, BIMI, and MTA-STS. Acquired by Red Sift, integrates with broader cybersecurity offerings.

- **[Mimecast DMARC Analyzer](https://www.mimecast.com/)**
  DMARC module within the Mimecast email security suite. Provides report analysis and enforcement guidance integrated with Mimecast's gateway.

- **[Proofpoint Email Fraud Defense](https://www.proofpoint.com/)**
  Email fraud defense with DMARC enforcement and supplier chain protection. Part of Proofpoint's broader email security ecosystem.

- **[Sendmarc](https://sendmarc.com/)**
  DMARC platform with a strong MSP focus and 90-day enforcement guarantee. Covers DMARC, SPF, DKIM, MTA-STS, and BIMI with hosted BIMI record management and VMC/CMC certificate purchasing assistance. Known for hands-on expert support during enforcement .

- **[URIports](https://www.uriports.com/)**
  Unified domain monitoring platform covering DMARC, TLS-RPT, CSP, DNS, and SSL/TLS certificates. Provides DMARC enforcement guidance and hosted MTA-STS. Pricing tiered by report volume and domain count .

- **[DMARCLY](https://dmarcly.com/)**
  DMARC monitoring and enforcement platform with SPF flattener and hosted DMARC records. Focused on simplifying DMARC for IT teams.

## Open-Source GitHub Projects

- **[DMARC Analyzer](https://github.com/dmarc-analyzer/dmarc-analyzer)**
  Comprehensive self-hosted DMARC monitoring platform for agencies and IT teams managing email authentication across many client domains. Ingests aggregate reports from a dedicated IMAP mailbox (rua= destination), parses XML reports, and displays sender identity, SPF/DKIM alignment, and enforcement progress. **Unlimited domains, no per-domain pricing.** Docker deployment with PostgreSQL. Mailbox credentials encrypted at rest. Apache-2.0 .

- **[DMARCus Analyzer](https://github.com/mmattavelli/dmarcus-app)**
  Flask-based web application for parsing, analyzing, and visualizing DMARC aggregate reports. Parses XML, GZIP, and ZIP formats. Extracts SPF/DKIM results, policy dispositions, source IPs, and identifies internal vs external senders. Features interactive dashboard with time-series charts, GeoIP integration, CSV/JSON export, and flat-file JSON storage (no external database required). Includes security hardening: CSRF protection, rate limiting, defusedxml for XXE prevention, and strict session security .

- **[DMARQ](https://github.com/christianlouis/dmarq)**
  Self-hosted DMARC aggregate report processor and dashboard. Supports DMARC aggregate reports, inbound RUF/failure reports, SMTP TLS/TLS-RPT reports, DMARC/SPF/DKIM DNS linting, MTA-STS, and BIMI. Features health scoring, sender reputation checks, Cloudflare integration for DNS remediation (with explicit operator confirmation), Apprise-based alerts (email/Slack/webhook), and Docker Compose deployment. Web-based setup wizard. Logto-based authentication .

- **[DmarcSrg](https://github.com/techsneeze/dmarcts-report-parser)**
  PHP parser, viewer, and summary report generator for incoming DMARC reports. View parsed reports in a table, identify issues through colors, filter by domain/month/reporting organization, view DKIM/SPF details, password-protected web interface, receive/process reports from mailboxes or local directories, upload reports via web UI, and generate weekly/monthly summary reports. Available in Debian repositories .

- **[dmarcts-report-parser](https://github.com/techsneeze/dmarcts-report-parser)**
  Perl-based DMARC report parser that stores reports in a MySQL/MariaDB database. Command-line tool for automated ingestion. Companion to DmarcSrg web viewer.

- **[Viesti-Reports](https://github.com/antedebaas/Viesti-Reports)**
  DMARC & SMTP-TLS reports processor and visualizer with BIMI file hosting. PHP-based, 95+ stars .

- **[Akila Audit DMARC](https://github.com/urian121/akila-audit-dmarc)**
  Python + Flask API for validating email authentication configuration: SPF, DMARC, DKIM, MX, DNSSEC, MTA-STS, TLS-RPT, BIMI. Uses checkdmarc and dkimpy. Features on-demand domain checking, continuous monitoring with PostgreSQL persistence, DNS record generation guidance, and optional AI summary via OpenAI. Frontend uses htmx .

- **[MailAuth](https://github.com/postalsys/mailauth)**
  Command-line utility and Node.js library for email authentication. Supports DKIM, SPF, DMARC, ARC, and BIMI validation. 121 stars, JavaScript .

- **[MailPolicyExplainer](https://github.com/rhymeswithmogul/MailPolicyExplainer)**
  PowerShell module to test and explain all facets of a domain's email records including SPF, DKIM, DMARC, and BIMI .

### Additional Strong Open-Source Options

- **Report Parsing & Storage**: **DMARC Analyzer** (PostgreSQL, unlimited domains), **DmarcSrg** (PHP + MySQL), **dmarcts-report-parser** (Perl + MySQL).
- **Validation Libraries**: **checkdmarc** (Python), **dkimpy** (Python DKIM), **mailauth** (Node.js).
- **BIMI Tooling**: **SVG Tiny PS converters** (php-svg-ps-converter, svgtinyps-cli) for BIMI-compliant logo preparation.
- **DNS Linting**: **MailPolicyExplainer** (PowerShell), **emaildnscheck** (Python).

**Frameworks for building custom systems**: Combine **DMARC Analyzer** for the core ingestion and dashboard, **checkdmarc** for real-time domain validation, **DmarcSrg** for PHP-based deployments, and **PostgreSQL** for persistence. Add **Apprise** for alert routing and **Cloudflare API** for DNS remediation.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Email authentication tools handle sensitive DNS and email flow data; ensure proper access controls and credential encryption.
- Self-hosted open-source solutions require an IMAP mailbox for receiving reports, database infrastructure, and ongoing maintenance. The license is free; the operational cost is yours.
