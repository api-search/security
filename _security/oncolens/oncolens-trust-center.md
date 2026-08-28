---
certifications:
- SOC 2
- HIPAA
- SOC 3
- ISO 27001
- HITRUST
- PCI DSS
- FedRAMP
description: OncoLens operates a real, publicly reachable SafeBase trust center on its own domain. It is the single most substantive machine-adjacent artifact the company publishes — 30+ security controls marked at full maturity, SOC 2 and HIPAA compliance entries, and gated report downloads. It carries no API, developer, or interoperability content.
kind: trust-center
layout: security
name: Oncolens Trust Center
name_suffix: Trust Center
overview: OncoLens maintains a public trust center documenting SOC 2, HIPAA, SOC 3, ISO 27001, HITRUST, PCI DSS, and FedRAMP compliance.
provider_name: OncoLens
provider_slug: oncolens
slug: oncolens-trust-center
source_filename: oncolens-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nprobe: true\nsource: https://trust.oncolens.com/\nurl: https://trust.oncolens.com/\nname: OncoLens Trust Center\ndescription: >-\n  OncoLens operates a real, publicly reachable SafeBase trust center on its own domain. It is\n  the single most substantive machine-adjacent artifact the company publishes — 30+ security\n  controls marked at full maturity, SOC 2 and HIPAA compliance entries, and gated report\n  downloads. It carries no API, developer, or interoperability content.\nplatform: SafeBase\nplatform_evidence: 'DNS CNAME: trust.oncolens.com -> oncolens.portals.safebase.io'\nplan: free\ncustom_domain: trust.oncolens.com\nprimary_domain: oncolens.com\nevidence:\n- source: https://trust.oncolens.com/\n  http_status: 200\n  content_type: text/html\n  bytes: 236247\n  method: >-\n    Read from the embedded __NEXT_DATA__ payload on the rendered page. NOTE for re-runs: a\n    curl request sending a full desktop-browser User-Agent is\
  \ answered with a Cloudflare\n    interactive challenge (HTTP 403, \"Just a moment...\"); a plain library User-Agent is\n    served the page (HTTP 200). The 403 is a bot-fingerprint edge policy, not an access wall.\n  keywords: [soc 2, hipaa, trust center, safebase]\ncertifications:\n- name: SOC 2\n  status: published\n  maturity: full\n  report_available: true\n  report_access: gated\n  report_note: >-\n    A \"SOC 2 Report\" document entry is enabled and carries attached files, but the files are\n    not shared publicly (isShared false) — access is request/NDA gated through SafeBase.\n    Report type (Type I vs Type II), auditor and period are not disclosed anonymously.\n- name: HIPAA\n  status: published\n  maturity: full\n  report_available: false\n  report_note: >-\n    The HIPAA compliance entry is enabled; the separate \"HIPAA Report\" document entry is\n    NOT enabled on this trust center.\n- name: SOC 3\n  status: not-published\n  note: The \"SOC 3 Report\" item exists in the\
  \ SafeBase template but is disabled.\n- name: ISO 27001\n  status: not-published\n- name: HITRUST\n  status: not-published\n  note: >-\n    Notable for a US oncology data platform — HITRUST CSF is the certification most often\n    requested of healthcare vendors handling PHI, and it is absent.\n- name: PCI DSS\n  status: not-published\n  note: Not applicable; OncoLens is not a payment surface.\n- name: FedRAMP\n  status: not-published\nsecurity_program:\n  penetration_testing:\n    published: true\n    maturity: full\n    report_access: gated\n  controls_published: 38\n  controls_at_full_maturity: 33\n  controls:\n  - Access Monitoring\n  - BC/DR\n  - Cloud Workload Protection\n  - Code of Ethics\n  - Critical Dependence\n  - Cyber Insurance\n  - DNS Filtering\n  - Data Access Level\n  - Data Backups\n  - Data Erasure\n  - Data Loss Prevention\n  - Data Privacy Officer\n  - Disk Encryption\n  - Effective Board Oversight\n  - Employee Privacy Training\n  - Encryption-at-rest\n  - Encryption-in-transit\n\
  \  - Endpoint Detection & Response\n  - Hosting\n  - Impact Level\n  - Infrastructure Security\n  - Pentest Report\n  - Physical Security\n  - Secure Development Training\n  - Security Information and Event Management\n  - Separate Production Environment\n  - Software Bill of Materials (SBOM)\n  - Software Development Lifecycle\n  - Third Party Dependence\n  - Threat Detection\n  - Virtual Private Cloud\n  - Vulnerability & Patch Management\n  - Web Application Firewall\n  - Zero Trust\n  subprocessors_published: true\ngaps:\n- >-\n  securityMailbox is null on the SafeBase org record, and no security.txt is served on any\n  OncoLens host — there is no published vulnerability-disclosure contact or policy despite a\n  full pentest program being advertised.\n- >-\n  The trust center's own \"Terms of Service\" and \"Privacy Policy\" document slots are disabled,\n  and no terms-of-service page exists on www.oncolens.com (probed /terms/, /terms-of-use/,\n  /terms-of-service/, /terms-and-conditions/\
  \ — all 404).\n- >-\n  No API, integration, or interoperability content appears anywhere in the trust center.\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oncolens/refs/heads/main/security/oncolens-trust-center.yml
summary_line: SOC 2, HIPAA, SOC 3, ISO 27001, HITRUST, PCI DSS, FedRAMP
tags:
- Company
- Healthcare
- Oncology
- Cancer Care
- Clinical Trials
- Health Data
- Real World Data
- Artificial Intelligence
- Analytics
- Clinical Workflow
- Cancer Registry
- Life Sciences
- SaaS
trust_url: https://trust.oncolens.com/
---
