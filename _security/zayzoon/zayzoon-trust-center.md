---
certification_count: 1
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Zayzoon Trust Center
name_suffix: Trust Center
overview: ZayZoon maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: ZayZoon
provider_slug: zayzoon
slug: zayzoon-trust-center
source_filename: zayzoon-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nsource: https://www.zayzoon.com/security\nurl: https://app.vanta.com/zayzoon/trust/3q6v6nbz0d1g20l1brgbhs\nname: ZayZoon Trust Center\nplatform: Vanta\nnote: >-\n  ZayZoon links a Vanta-hosted Trust Center from the footer of its own security page.\n  The Vanta page returns HTTP 200 but renders client-side, so its document list could\n  not be read anonymously; the certifications below are taken from ZayZoon's own\n  first-party security page, which is server-rendered.\ncertifications:\n- name: SOC 2 Type II\n  scope: security, availability, confidentiality\n  holder: ZayZoon\n  status: attested\n  availability: on request\n  evidence: https://www.zayzoon.com/security\n  quote: >-\n    \"ZayZoon has a SOC 2 Type II report. Our SOC 2 report attests to the controls we\n    have in place governing the availability, confidentiality, and security of customer\n    data as they map to Trust Service Principles (TSPs) established\
  \ by the American\n    Institute of Certified Public Accountants (AICPA).\"\ninherited_certifications:\n- name: ISO 27001\n  holder: cloud infrastructure providers (AWS, GCP)\n  note: >-\n    NOT held by ZayZoon. The security page states \"ZayZoon products are hosted with\n    cloud infrastructure providers with SOC 2 Type II and ISO 27001 certifications\".\n    Recorded separately so it is never credited to ZayZoon itself.\n  evidence: https://www.zayzoon.com/security\nsecurity_practices:\n- practice: in-transit encryption\n  detail: TLS 1.2 or above, 2,048-bit or better keys\n- practice: third-party penetration testing\n  detail: performed several times a year against products and product infrastructure\n- practice: vulnerability assessment\n  detail: recurring static code analysis and infrastructure vulnerability scans\n- practice: web application firewall, network firewalling, DDoS prevention\n- practice: patch management with server-level instrumentation\n- practice: defined security\
  \ incident response process\nregulatory:\n- item: NMLS ID 2635812\n  source: https://www.zayzoon.com/security\n  note: Nationwide Multistate Licensing System identifier published in the site footer.\nnot_found:\n- PCI DSS\n- HIPAA\n- FedRAMP\n- ISO 27001 held by ZayZoon itself\n- a published bug bounty program\nchecked: '2026-09-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayzoon/refs/heads/main/security/zayzoon-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Earned Wage Access
- On-Demand Pay
- Payroll
- Human Resources
- Employee Benefits
- Financial Wellness
- Fintech
- Payments
- Embedded Finance
trust_url: https://app.vanta.com/zayzoon/trust/3q6v6nbz0d1g20l1brgbhs
---
