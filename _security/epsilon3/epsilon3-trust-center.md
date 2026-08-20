---
certifications:
- SOC 2 Type II
- FedRAMP High Authorization
- NIST SP 800-171
- DFARS 252.204-7012
- CMMC
- ITAR
- EAR
description: ''
kind: trust-center
layout: security
name: Epsilon3 Trust Center
name_suffix: Trust Center
overview: Epsilon3 maintains a public trust center documenting SOC 2 Type II, FedRAMP High Authorization, NIST SP 800-171, DFARS 252.204-7012, CMMC, ITAR, and EAR compliance.
provider_name: Epsilon3
provider_slug: epsilon3
slug: epsilon3-trust-center
source_filename: epsilon3-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nprobe_note: >-\n  0-working/probe-security-programs.py returned trust=none because trust.epsilon3.io is a\n  Vanta-hosted single-page app - the served HTML is 7,201 bytes containing only the title\n  \"Epsilon3 Trust Center\", with every certification rendered client-side, so the probe's\n  keyword threshold could not be met. The trust center is nonetheless real and reachable\n  (HTTP 200), and Epsilon3's own security page names the certifications server-side. This\n  file is written from that server-side evidence, not from the JS-rendered page.\nurl: https://trust.epsilon3.io/\nhttp_status: 200\nprovider: Vanta\ncontent_rendering: client-side (JS); no certification text in the served HTML\nsource_page: https://www.epsilon3.io/security\ncertifications:\n- SOC 2 Type II\n- FedRAMP High Authorization\n- NIST SP 800-171\n- DFARS 252.204-7012\n- CMMC\n- ITAR\n- EAR\ncontrols:\n- {control: encryption-in-transit, detail: TLS\
  \ 1.3}\n- {control: encryption-at-rest, detail: AES-256}\n- {control: access-control, detail: Role-Based Access Control to restrict access to\n    classified or sensitive data}\n- {control: identity, detail: Single Sign-On (SSO) and Multi-Factor Authentication (MFA)}\n- {control: auditability, detail: one-click audit bundle export for internal reviews and\n    regulatory audits}\n- {control: continuity, detail: dual-region clouds plus an offline mode}\nhosting: AWS GovCloud\ndeployment_models:\n- compliant cloud (AWS GovCloud, FedRAMP High)\n- on-premises\n- hybrid and international\n- classified environments\nai_data_posture: >-\n  AI features are opt-in and under user control; Epsilon3 states its contracts prevent\n  customer data being used to train models.\nevidence:\n- {source: 'https://www.epsilon3.io/security', http_status: 200, keywords: [SOC 2 Type II,\n      FedRAMP High, NIST 800-171, DFARS 252.204-7012, CMMC, ITAR, EAR, AWS GovCloud,\n      TLS 1.3, AES-256, Vanta trust report]}\n\
  - {source: 'https://trust.epsilon3.io/', http_status: 200, keywords: [Epsilon3 Trust Center],\n  note: title only - remainder is JS-rendered}\ngaps:\n- No public vulnerability disclosure or responsible disclosure policy. The strings\n  \"disclosure\", \"bug bounty\", \"security@\" and \"penetration\" do not appear on\n  www.epsilon3.io/security, no /.well-known/security.txt is served on any Epsilon3 host,\n  and no HackerOne/Bugcrowd/Intigriti program was found. No Security pointer is claimed in\n  apis.yml as a result.\n- Certification reports themselves are behind the Vanta trust center, which requires\n  interaction to reach; nothing is downloadable anonymously.\n- ISO 27001 is not among the named certifications.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon3/refs/heads/main/security/epsilon3-trust-center.yml
summary_line: SOC 2 Type II, FedRAMP High Authorization, NIST SP 800-171, DFARS 252.204-7012, CMMC, ITAR, EAR
tags:
- Company
- Aerospace
- Space
- Defense
- Manufacturing
- Procedures
- Workflows
- Inventory
- Telemetry
- Test Management
- Project Management
- MCP
trust_url: https://trust.epsilon3.io/
---
