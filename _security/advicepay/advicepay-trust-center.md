---
certification_count: 2
certifications:
- SOC 2 Type II
- PCI SAQ A
description: ''
kind: trust-center
layout: security
name: Advicepay Trust Center
name_suffix: Trust Center
overview: AdvicePay maintains a public trust center documenting SOC 2 Type II and PCI SAQ A compliance.
provider_name: AdvicePay
provider_slug: advicepay
slug: advicepay-trust-center
source_filename: advicepay-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nprobe: true\nsource: https://advicepay.com/security/\nurl: https://advicepay.com/security/\nstyle: security-page\nnote: >-\n  AdvicePay has no dedicated trust portal (trust.advicepay.com does not resolve) — the compliance\n  posture is published as a section of its own website. Enriched by hand from the page after the\n  mechanical probe recorded only \"SOC 2\"; the detail below is quoted from that page.\ncertifications:\n- id: soc2-type-ii\n  name: SOC 2 Type II\n  first_party: true\n  auditor: KirkpatrickPrice\n  cadence: annual\n  scope: Reporting controls relating to security and availability.\n  report_available: not stated\n- id: pci-saq-a\n  name: PCI SAQ A\n  first_party: true\n  cadence: annual\n  scope: >-\n    Self-Assessment Questionnaire A, performed as required by AdvicePay's processing partner\n    Stripe. AdvicePay states it does not store, process or transmit cardholder data — Stripe\n    performs all cardholder-data\
  \ functions — which is what makes SAQ A the applicable instrument.\ncontrols:\n- id: penetration-testing\n  description: Annual independent third-party penetration tests of the platform.\n- id: encryption-in-transit\n  description: HTTPS exclusively for all client and advisor traffic. Confirmed by probe — TLS 1.3\n    with HSTS (max-age 31536000) on advicepay.com and docs.advicepay.com.\n- id: mfa\n  description: The pricing comparison lists \"Required MFA\" as a data and security feature.\n- id: audit-logs\n  description: Audit logs and email logs, listed on the pricing comparison.\n- id: status-transparency\n  description: >-\n    Maintenance, incidents and operational security issues are reported on\n    https://status.advicepay.com/.\nvendor_certifications_inherited:\n  note: >-\n    THESE ARE NOT ADVICEPAY'S OWN ATTESTATIONS. The security page also lists its vendors'\n    certifications, which is common practice but easy to misread as first-party. Recorded\n    separately so no reader\
  \ or scorer credits them to AdvicePay.\n  vendors:\n  - vendor: Amazon Web Services\n    role: infrastructure hosting\n    certifications:\n    - ISO 27001\n    - ISO 27017\n    - ISO 27018\n    - SOC 1/SSAE 16/ISAE 3402\n    - SOC 2\n    - SOC 3\n    - PCI DSS Level 1\n  - vendor: Stripe\n    role: payment processing\n    certifications:\n    - PCI DSS Service Provider Level 1\n    - SOC 2 Type II (annual)\nlegal:\n  terms_of_use: https://advicepay.com/terms-of-use/\n  privacy_policy: https://advicepay.com/privacy-policy\nevidence:\n- source: https://advicepay.com/security/\n  status: 200\n  keywords:\n  - soc 2 type ii\n  - kirkpatrickprice\n  - pci saq a\n  - penetration tests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advicepay/refs/heads/main/security/advicepay-trust-center.yml
summary_line: SOC 2 Type II, PCI SAQ A
tags:
- Financial Services
- Payments
- Billing
- Invoicing
- Financial Planning
- Wealth Management
- Subscriptions
- eSignature
- Compliance
- FinTech
trust_url: https://advicepay.com/security/
---
