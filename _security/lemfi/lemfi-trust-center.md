---
certifications:
- SOC 2 Type II
- PCI DSS
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Lemfi Trust Center
name_suffix: Trust Center
overview: LemFi maintains a public trust center documenting SOC 2 Type II, PCI DSS, ISO 27001, and GDPR compliance.
provider_name: LemFi
provider_slug: lemfi
slug: lemfi-trust-center
source_filename: lemfi-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://trust.lemfi.com/\nurl: https://trust.lemfi.com/\nhttp_status: 200\nhosted_by: Secureframe\nhosted_by_note: >-\n  trust.lemfi.com is a CNAME to lemfi.secureframetrust.com — the trust center is a\n  Secureframe-hosted single-page app. Every /.well-known/* and /openapi.json path on\n  this host returns HTTP 200 with the same 151KB HTML shell, so it is an SPA catch-all,\n  not a document surface. Recorded as a miss for well-known purposes.\ncertifications:\n- name: SOC 2 Type II\n  evidence: Listed on the trust center with a SOC 2 Type II Certificate and a Bridge Letter\n  document_access: request-required\n- name: PCI DSS\n  level: Level 1\n  evidence: Listed on the trust center with a PCI DSS Certificate and PCI DSS AOC Report\n  document_access: request-required\n- name: ISO 27001\n  evidence: Listed on the trust center as a compliance framework\n  document_access: request-required\n- name: GDPR\n  evidence: Listed on\
  \ the trust center as a compliance framework\n  document_access: public\ndocuments:\n  request_required:\n  - SOC 2 Type II Certificate\n  - SOC 2 Type II Bridge Letter\n  - PCI DSS Certificate\n  - PCI DSS AOC Report\n  public:\n  - Privacy Policy\n  - Terms of Service\ncontrol_families:\n  change_management:\n  - Configuration and Asset Management Policy\n  - Environment segregation\n  - Restricted use of production data\n  - Change Management Policy\n  availability:\n  - Business Continuity and Disaster Recovery Policy\n  - Annual backup restoration testing\n  organizational:\n  - Acceptable Use Policy\n  - Information Security Policy\n  - Cybersecurity insurance\n  confidentiality:\n  - Data Classification Policy\n  - Data Retention and Disposal Policy\n  vulnerability_management:\n  - Annual third-party penetration testing\n  - Vulnerability and Patch Management Policy\n  incident_response:\n  - Incident Response Plan\n  - Periodic tabletop exercises\n  risk_assessment:\n  - Vendor\
  \ Risk Management Policy\n  - Risk Assessment and Treatment Policy\n  network_security:\n  - Network Security Policy\n  access_security:\n  - Complex passwords with MFA\n  - Encryption in transit, TLS 1.2+\n  - Restricted SSH and key access to production\n  data_protection:\n  - AES-256 encryption at rest\n  - AWS infrastructure hosting\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemfi/refs/heads/main/security/lemfi-trust-center.yml
summary_line: SOC 2 Type II, PCI DSS, ISO 27001, GDPR
tags:
- Company
- Financial Services
- Fintech
- Payments
- Remittances
- Cross-Border Payments
- Money Transfer
- Consumer Finance
- Mobile Banking
- eSIM
trust_url: https://trust.lemfi.com/
---
