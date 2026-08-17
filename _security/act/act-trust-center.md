---
api_specs:
- filename: v1
  format: yaml
  label: Act! Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://apimta.act.com/act.web.api/swagger/docs/v1
certifications:
- SOC 2
- SOC 3
- ISO 27001
- PCI DSS
- HIPAA
- FedRAMP
description: 'Act! has no trust-center portal — no Vanta/Drata/SafeBase page, no self-service report request. What it publishes is a downloadable Security and Privacy whitepaper that names its audits and its hosting posture, plus a marketing page explaining what SOC 2 and SOC 3 mean. The audit reports themselves are gated: the SOC 2 report requires an NDA and the SOC 3 report is "available on request".'
kind: trust-center
layout: security
name: Act Trust Center
name_suffix: Trust Center
overview: Act! CRM maintains a public trust center documenting SOC 2, SOC 3, ISO 27001, PCI DSS, HIPAA, and FedRAMP compliance.
provider_name: Act! CRM
provider_slug: act
slug: act-trust-center
source_filename: act-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.act.com/uploads/act_security_privacy_whitepaper.pdf (Act! Products\n  Security and Privacy whitepaper, 7 pages, fetched 2026-08-13),\n  https://www.act.com/resources/soc-compliance/ and\n  https://www.act.com/legal/privacy-policy/.\ndescription: >-\n  Act! has no trust-center portal — no Vanta/Drata/SafeBase page, no\n  self-service report request. What it publishes is a downloadable Security and\n  Privacy whitepaper that names its audits and its hosting posture, plus a\n  marketing page explaining what SOC 2 and SOC 3 mean. The audit reports\n  themselves are gated: the SOC 2 report requires an NDA and the SOC 3 report is\n  \"available on request\".\ntrust_center_portal: false\nportal_url: null\ndocuments:\n  - name: Act! Products Security and Privacy whitepaper\n    url: https://www.act.com/uploads/act_security_privacy_whitepaper.pdf\n    http_status: 200\n    fetched: '2026-08-13'\n    pages: 7\n    note:\
  \ >-\n      Marked \"Confidential & Proprietary\" in its own footer while being served\n      unauthenticated from the site footer link.\n  - name: SOC Compliance resources\n    url: https://www.act.com/resources/soc-compliance/\n    http_status: 200\n    fetched: '2026-08-13'\n    note: >-\n      Educational — explains the difference between SOC 2 and SOC 3 and links a\n      free PDF. It does NOT itself assert an Act! certification; the\n      certification claims live in the whitepaper above.\n  - name: Act! Global Privacy Policy\n    url: https://www.act.com/legal/privacy-policy/\n  - name: Terms of Service\n    url: https://www.act.com/legal/terms-of-service/\ncertifications:\n  - name: SOC 2\n    status: claimed\n    scope: Act! Premium Cloud\n    evidence: >-\n      \"This entire process has been validated by the SOC 2 audit process\"; Act!'s\n      vendor selection process \"has been evaluated as SOC 2 compliant\"; database\n      access during support follows \"a SOC 2-compliant\
  \ process\"; SOC 2-compliant\n      Emergency Response and Business Continuity processes.\n    report_access: NDA required\n    auditor: not named\n    period: not stated\n  - name: SOC 3\n    status: claimed\n    scope: Act! Premium Cloud\n    evidence: '\"the SOC 3 Audit Report (available on request)\"'\n    report_access: available on request\n    note: >-\n      A SOC 3 report is designed for public distribution. Act! gates it behind a\n      request anyway, which is the opposite of how the report type is meant to\n      work and is the single easiest credibility upgrade available here.\n  - name: ISO 27001\n    status: not claimed\n  - name: PCI DSS\n    status: not claimed\n    note: >-\n      Act! Payments accepts card payments, but no PCI attestation is published\n      in the whitepaper or on the payments product page.\n  - name: HIPAA\n    status: not claimed\n  - name: FedRAMP\n    status: not claimed\nsecurity_posture_published:\n  hosting: Amazon Web Services; end-user data-center\
  \ region defaults from billing postal code. Act! stores no customer databases at its office locations.\n  tenancy: Each customer database is stored and backed up as an independent database.\n  encryption_in_transit: TLS 1.2 (whitepaper states \"currently (July 2023), we support TLS 1.2\")\n  encryption_at_rest: SHA 256 (as worded in the whitepaper)\n  backups: Daily, encrypted, stored off the database server.\n  mfa: Available on Act! Premium Cloud; enforced on the AWS Management Console.\n  endpoint_protection: Anti-virus/endpoint protection on every server, updated daily.\n  monitoring: 24/7 threat monitoring in partnership with Rapid7; engineer on duty outside business hours.\n  privileged_access: AWS console access limited to teams of four or fewer screened employees, restricted to the internal network or VPN, reviewed daily by a Director-level role.\n  support_access: Act! employees do not access a customer database without documented customer consent.\nfindings:\n  - >-\n    The\
  \ whitepaper's encryption statements are dated July 2023 and stop at TLS\n    1.2. Live probing on 2026-08-13 found www.act.com and developer.act.com\n    negotiating TLS 1.3, but the API host apimta.act.com negotiating TLS 1.2 —\n    so the API is the laggard, and the published document has not been revised\n    in three years. See security/act-domain-security.yml.\n  - >-\n    \"encrypted at rest, SHA 256\" describes a hash, not a cipher. The intended\n    claim is presumably AES-256; as written the statement does not say what it\n    means.\n  - No ISO 27001 and no PCI DSS attestation published despite shipping a payments product.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/security/act-trust-center.yml
summary_line: SOC 2, SOC 3, ISO 27001, PCI DSS, HIPAA, FedRAMP
tags:
- CRM
- Customer Relationship Management
- Marketing Automation
- Contact Management
- Sales
- Opportunity Management
- OData
- Small Business
trust_url: ''
---
