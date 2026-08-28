---
certifications:
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Payzen Trust Center
name_suffix: Trust Center
overview: PayZen maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: PayZen
provider_slug: payzen
slug: payzen-trust-center
source_filename: payzen-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://payzen.com/payzen-compliance/\ntrust_center:\n  url: https://app.vanta.com/payzen/trust\n  platform: Vanta\n  status: 200\n  note: >-\n    Linked from PayZen's own Security & Compliance page as \"Go to the trust portal\". The\n    Vanta portal answers 200 but serves a client-side shell (~5KB, no server-rendered\n    content), so the certification list below is read from PayZen's own compliance page\n    rather than from the portal HTML.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  scope: PayZen platform\n  evidence: https://payzen.com/payzen-compliance/\n  note: >-\n    PayZen announced SOC 2 Type II certification publicly in 2022; the compliance page\n    carries a \"SOC2 CERTIFICATION\" section. Report availability is not stated publicly.\n- name: HIPAA\n  status: compliant\n  scope: patient and provider information handled by the platform\n  evidence: https://payzen.com/payzen-compliance/\n  note:\
  \ >-\n    Self-attested on the compliance page (\"our systems are built to meet strict HIPAA\n    requirements\"). HIPAA has no certification body; treat as a program claim, not a cert.\nlicensing:\n- registry: NMLS (Nationwide Multistate Licensing System)\n  entity: PayZen LLC\n  identifier: '2591891'\n  evidence: https://payzen.com/payzen-compliance/\nnot_found:\n- ISO 27001\n- PCI DSS\n- HITRUST\n- FedRAMP\n- published subprocessor list\n- named security contact / security@ address\n- vulnerability disclosure or bug bounty policy\nevidence:\n- url: https://payzen.com/payzen-compliance/\n  status: 200\n  kind: provider compliance page\n- url: https://app.vanta.com/payzen/trust\n  status: 200\n  kind: Vanta trust portal (JS-rendered shell)\n- url: https://payzen.com/.well-known/security.txt\n  status: 404\n  kind: negative probe\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payzen/refs/heads/main/security/payzen-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Company
- Payments
- Healthcare
- Patient Financing
- Revenue Cycle Management
- Lending
- Fintech
- Electronic Health Records
trust_url: ''
---
