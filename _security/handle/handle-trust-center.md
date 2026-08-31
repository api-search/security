---
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Handle Trust Center
name_suffix: Trust Center
overview: Handle maintains a public trust center documenting SOC 2 Type 1 and SOC 2 Type 2 compliance.
provider_name: Handle
provider_slug: handle
slug: handle-trust-center
source_filename: handle-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://www.handle.com/security-and-trust/\nprobe: true\nurl: https://trust.handle.com/\nplatform: Vanta\ncertifications:\n- SOC 2 Type 1\n- SOC 2 Type 2\npractices:\n- Regular penetration testing and security audits\n- Continuous compliance/policy monitoring\nreport_access: >-\n  The SOC 2 report is gated — \"Request Report\" links to the Vanta trust center at https://trust.handle.com/,\n  which requires a request/NDA flow.\ncontrol_families:\n- name: Infrastructure security\n  controls: 16\n- name: Organizational security\n  controls: 10\n- name: Product security\n  controls: 5\n- name: Internal security procedures\n  controls: 18\n- name: Data and privacy\n  controls: 9\nevidence:\n- source: https://www.handle.com/security-and-trust/\n  http_status: 200\n  keywords: [soc 2 type 1, soc 2 type 2, compliance monitoring, penetration testing, trust]\n- source: https://trust.handle.com/\n  http_status: 200\n  note: >-\n    Vanta-hosted\
  \ trust report. The served HTML is a client-side shell whose only text is\n    \"Handle Inc Trust Center\"; the control and certification detail renders from assets.vanta.com\n    scripts, so the certification list above was read from the provider's own\n    /security-and-trust/ page instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handle/refs/heads/main/security/handle-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2
tags:
- Company
- Construction
- Construction Finance
- Lien Management
- Lien Waivers
- Accounts Receivable
- Credit Management
- Payments
- B2B Payments
- Payment Compliance
- ERP Integrations
- Collection
- Financial Operations
- Material Suppliers
- Equipment Dealers
trust_url: https://trust.handle.com/
---
