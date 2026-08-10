---
certifications:
- SOC 1 Type II
- SOC 2 Type II
- PCI DSS
- GDPR
- CCPA
- Vendor Security Alliance (VSA)
description: ''
kind: trust-center
layout: security
name: Mesh Payments Trust Center
name_suffix: Trust Center
overview: Mesh Payments maintains a public trust center documenting SOC 1 Type II, SOC 2 Type II, PCI DSS, GDPR, CCPA, and Vendor Security Alliance (VSA) compliance.
provider_name: Mesh Payments
provider_slug: mesh-payments
slug: mesh-payments-trust-center
source_filename: mesh-payments-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nprobe_result: no trust.meshpayments.com or security.meshpayments.com host exists (NXDOMAIN),\n  and /trust and /security both 404; the compliance posture is published on a single\n  marketing-path security page instead of a dedicated trust center.\nurl: https://meshpayments.com/security-is-our-priority/\ndedicated_trust_center: false\ncertifications:\n- name: SOC 1 Type II\n  auditor: KPMG\n  cadence: annual external audit\n- name: SOC 2 Type II\n  auditor: KPMG\n  cadence: annual external audit\n  note: covers security, availability and confidentiality; continuous compliance monitoring\n    with Drata\n- name: PCI DSS\n  level: Level 1 Service Provider\n- name: GDPR\n  kind: regulatory compliance\n- name: CCPA\n  kind: regulatory compliance\n- name: Vendor Security Alliance (VSA)\n  kind: core self-assessment completed\ncontrols_published:\n- encryption at rest with AES-256\n- encryption in transit with TLS 1.2+\n- multi-factor\
  \ authentication required\n- SAML SSO with passwordless access\n- continuous penetration testing\n- static and dynamic code analysis plus software composition analysis (SCA)\n- zero-trust VPN for remote access\n- documented incident response procedures\n- daily AWS backups with disaster recovery\n- least-privilege access with audit logging\n- EDR malware detection\n- annual security awareness training\nreport_access: 'SOC report detail is available on request via https://meshpayments.com/contact-us/\n  - not self-serve.'\ngaps:\n- No self-serve trust portal (Vanta/Drata/SafeBase style) and no downloadable evidence\n  under NDA; reports are request-only through a contact form.\n- No public status page or uptime history was found on any Mesh host, so the availability\n  half of the SOC 2 claim is not independently observable.\nevidence:\n- source: https://meshpayments.com/security-is-our-priority/\n  http_status: 200\n  keywords:\n  - soc 1\n  - soc 2 type ii\n  - pci dss\n  - gdpr\n  -\
  \ ccpa\n  - kpmg\n  - penetration testing\n- source: https://meshpayments.com/blog/mesh-payments-is-soc-2-certified/\n  http_status: 200\n  keywords:\n  - soc 2\n  - kpmg\n  - drata\n- source: https://trust.meshpayments.com/\n  http_status: 0\n  note: DNS does not resolve\nx-evidence:\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-payments/refs/heads/main/security/mesh-payments-trust-center.yml
summary_line: SOC 1 Type II, SOC 2 Type II, PCI DSS, GDPR, CCPA, Vendor Security Alliance (VSA)
tags:
- Company
- Payments
- Spend Management
- Expense Management
- Corporate Cards
- Travel
- Accounts Payable
- Fintech
- Card Issuing
- Accounting Automation
trust_url: https://meshpayments.com/security-is-our-priority/
---
