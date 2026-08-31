---
certifications:
- ISO/IEC 27001
- ISO/IEC 27701
- ISO/IEC 27018
- SOC 1 Type 2
- SOC 2 Type 2
- SOC 3
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Simetrik Trust Center
name_suffix: Trust Center
overview: Simetrik maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27701, ISO/IEC 27018, SOC 1 Type 2, SOC 2 Type 2, SOC 3, and PCI DSS compliance.
provider_name: Simetrik
provider_slug: simetrik
slug: simetrik-trust-center
source_filename: simetrik-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://trust.simetrik.com/ (HTTP 200), https://simetrik.com/security/ (HTTP 200),\n  https://simetrik.com/information-security-privacy-policy/ (HTTP 200),\n  https://simetrik.com/data-privacy-treatment-policy/ (HTTP 200), https://docs.simetrik.com/mcp/data-handling,\n  and a DNS lookup of trust.simetrik.com, 2026-08-27.\nnote: >-\n  probe-security-programs.py returned trust=none for this provider. That was a false negative: the\n  trust center is served from a CNAME subdomain (trust.simetrik.com ->\n  667b5a6ebb4f7b57d3197659.cname.vantatrust.com) whose body is a JavaScript shell, so an automated\n  content probe finds no certification strings. The certifications below are read from Simetrik's own\n  first-party security page, which names them in prose, not from the trust center itself.\ntrust_center:\n  published: true\n  url: https://trust.simetrik.com/\n  http_status: 200\n  title: Simetrik Trust Center\n  provider:\
  \ Vanta\n  provider_evidence: trust.simetrik.com is a CNAME to 667b5a6ebb4f7b57d3197659.cname.vantatrust.com\n  content_readable: false\n  content_note: >-\n    The page returns a 7 KB HTML shell and renders its content client-side, so the certification list,\n    document requests and subprocessor inventory are not machine-readable from the served body. Access\n    to actual audit reports is the usual Vanta gated flow (request + NDA), not an open download.\n  linked_from: Site header and footer navigation on simetrik.com, labelled \"Trust Center\".\ncertifications:\n- name: ISO/IEC 27001\n  domain: Information security management\n  status: claimed\n- name: ISO/IEC 27701\n  domain: Privacy information management\n  status: claimed\n- name: ISO/IEC 27018\n  domain: Protection of PII in public clouds\n  status: claimed\n- name: SOC 1 Type 2\n  domain: Controls relevant to financial reporting\n  status: claimed\n- name: SOC 2 Type 2\n  domain: Security, availability, confidentiality and\
  \ privacy\n  status: claimed\n- name: SOC 3\n  domain: General-use report\n  status: claimed\n- name: PCI DSS\n  domain: Payment card data handling\n  status: claimed\ncertification_evidence: >-\n  All seven are named verbatim in the Compliance FAQ on https://simetrik.com/security/. `status:\n  claimed` throughout because no certificate number, auditor name, report date or scope statement is\n  published on any public page - the evidence sits behind the trust center. This is normal for the\n  category and is recorded as a provenance fact, not a doubt about the certifications.\npublished_policies:\n- name: Information Security & Privacy Policy\n  url: https://simetrik.com/information-security-privacy-policy/\n  http_status: 200\n  covers: >-\n    Risk-based protection of information assets, the confidentiality/integrity/availability\n    principles, shared-responsibility culture, training and awareness, and internal incident reporting\n    by employees, contractors and third parties.\n\
  - name: Data Treatment Policy\n  url: https://simetrik.com/data-privacy-treatment-policy/\n  http_status: 200\n- name: Privacy Notice\n  url: https://simetrik.com/privacy-notice/\n  http_status: 200\n- name: Cookie Policy\n  url: https://simetrik.com/cookie-policy/\n- name: Code of Ethics (employees)\n  url: https://simetrik.com/legal/code-of-ethics-employees/\n- name: Code of Ethics (third parties)\n  url: https://simetrik.com/legal/code-of-ethics-third-parties/\ntechnical_controls_published:\n- Encryption in transit on all external and internal communications.\n- Encryption at rest for all stored data.\n- Least-privilege access.\n- Defence in depth.\n- >-\n  PAN truncation at the agent boundary - the MCP server sends only the first six and last four digits\n  of a card number, matching the masking the web app shows on screen.\n- Every MCP call is authenticated, authorized and logged, acting as the signed-in user.\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n\
  \  security_txt_note: >-\n    /.well-known/security.txt returns 403 on simetrik.com, 404 on docs.simetrik.com and\n    mcp.us.simetrik.com, and a shell-installer body on cli.simetrik.com. No RFC 9116 file is served on\n    any host.\n  bug_bounty: false\n  bug_bounty_note: hackerone.com/simetrik and bugcrowd.com/simetrik both return 404.\n  disclosure_page: false\n  security_contact: null\n  note: >-\n    HONEST GAP. Simetrik publishes a formal information security policy and a full certification set,\n    but no external vulnerability disclosure path - no security.txt, no /security/disclosure page, no\n    published security@ address, no bug bounty. The incident reporting described in the policy is\n    internal, aimed at employees, contractors and third parties, not at outside researchers. For a\n    platform holding reconciliation data for banks, PSPs, issuers and acquirers, a served\n    /.well-known/security.txt would be the single cheapest fix available.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simetrik/refs/heads/main/security/simetrik-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27701, ISO/IEC 27018, SOC 1 Type 2, SOC 2 Type 2, SOC 3, PCI DSS
tags:
- Company
- Reconciliation
- Financial Operations
- Payments
- Accounting
- Fintech
- Financial Close
- Data Integration
- Agents
- MCP
- Latin America
trust_url: ''
---
