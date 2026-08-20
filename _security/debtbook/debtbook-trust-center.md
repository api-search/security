---
certifications:
- SOC 1 Type 1
- SOC 1 Type 2
- SOC 2 Type 1
- SOC 2 Type 2
- CSA STAR Level One
description: ''
kind: trust-center
layout: security
name: Debtbook Trust Center
name_suffix: Trust Center
overview: DebtBook maintains a public trust center documenting SOC 1 Type 1, SOC 1 Type 2, SOC 2 Type 1, SOC 2 Type 2, and CSA STAR Level One compliance.
provider_name: DebtBook
provider_slug: debtbook
slug: debtbook-trust-center
source_filename: debtbook-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://trust.debtbook.com/\nprobe: true\nurl: https://trust.debtbook.com/\nplatform: SecurityPal (trust.debtbook.com is a CNAME to debtbook.securitypal.com)\nsecurity_page: https://www.debtbook.com/security\ncertifications:\n- SOC 1 Type 1\n- SOC 1 Type 2\n- SOC 2 Type 1\n- SOC 2 Type 2\n- CSA STAR Level One\ndocuments:\n- name: SOC bridge letters\n  cadence: quarterly\n  access: available from the Trust Center Documents section\nposture:\n- Recognized security frameworks, continuous monitoring and regular third-party assessments\n  (per https://www.debtbook.com/security)\n- Audit reports, certifications, security policies and compliance documentation are\n  centralized in the trust center rather than published on the marketing site\ngaps:\n- No ISO 27001 certification named\n- No PCI DSS certification named\n- No HIPAA attestation named (notable given the healthcare vertical the platform serves)\n- No FedRAMP authorization\
  \ named (notable given the state/local government vertical)\n- Certification artifacts are gated behind trust-center access rather than published\n  openly\nevidence:\n- source: https://trust.debtbook.com/\n  http_status: 200\n  keywords:\n  - soc 1\n  - soc 2\n  - csa star\n  - trust center\n  fetched: '2026-08-04'\n- source: https://www.debtbook.com/security\n  http_status: 200\n  keywords:\n  - trust center\n  - third-party assessments\n  - continuous monitoring\n  fetched: '2026-08-04'\nx-evidence:\n  fetched: '2026-08-04'\n  note: the mechanical probe returned no hit because trust.debtbook.com renders client-side;\n    the page was fetched and read directly to confirm the named certifications.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debtbook/refs/heads/main/security/debtbook-trust-center.yml
summary_line: SOC 1 Type 1, SOC 1 Type 2, SOC 2 Type 1, SOC 2 Type 2, CSA STAR Level One
tags:
- Company
- Treasury Management
- Government
- Public Finance
- Debt Management
- Cash Management
- Accounting
- Lease Accounting
- Investment Management
- Non-Profit
- Higher Education
- Healthcare
- Software-as-a-Service
trust_url: https://trust.debtbook.com/
---
