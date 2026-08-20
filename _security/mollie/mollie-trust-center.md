---
api_specs:
- filename: mollie-openapi-original.yml
  format: yaml
  label: Mollie API
  slug: mollie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/openapi/mollie-openapi-original.yml
certifications:
- SOC 2 Type 2
- PCI-DSS Level 1
- ISAE 3402 Type 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Mollie Trust Center
name_suffix: Trust Center
overview: Mollie maintains a public trust center documenting SOC 2 Type 2, PCI-DSS Level 1, ISAE 3402 Type 2, and GDPR compliance.
provider_name: Mollie
provider_slug: mollie
slug: mollie-trust-center
source_filename: mollie-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://www.mollie.com/security\nnote: >-\n  Mollie does not run a dedicated trust-center subdomain — trust.mollie.com does not\n  resolve and www.mollie.com/trust and /compliance both return 404. The security page at\n  www.mollie.com/security is the published trust surface and names the attestations below.\ncertifications:\n- name: SOC 2 Type 2\n  detail: Security, availability and confidentiality controls independently assessed against\n    the AICPA Trust Services Criteria.\n- name: PCI-DSS Level 1\n  detail: Highest security tier for card payment processing, validated through an Attestation\n    of Compliance (AoC). Mollie Components let merchants stay within PCI-DSS SAQ-A.\n- name: ISAE 3402 Type 2\n  detail: Annual external audit providing independent assurance of operational controls and\n    integrity.\n- name: GDPR\n  detail: Data encryption and handling described on the security page; privacy statement\
  \ at\n    https://www.mollie.com/legal/privacy.\nregulatory:\n- regulator: De Nederlandsche Bank (DNB)\n  status: Licensed and supervised financial / e-money institution (Netherlands)\n- regulator: UK Financial Conduct Authority (FCA)\n  status: Licensed and supervised (United Kingdom)\nprograms:\n  responsible_disclosure: https://www.mollie.com/legal/responsible-disclosure\n  bug_bounty: https://hackerone.com/mollie\n  acknowledgments: https://hackerone.com/mollie/thanks\n  security_contact: security@mollie.com\n  pgp_key: https://www.mollie.com/security.aexpk\nlegal:\n  privacy: https://www.mollie.com/legal/privacy\n  user_agreement: https://www.mollie.com/legal/user-agreement\n  legal_index: https://www.mollie.com/legal\nevidence:\n- source: https://www.mollie.com/security\n  keywords: [soc 2 type 2, pci-dss level 1, isae 3402 type 2, dnb, fca, gdpr]\n- source: well-known/mollie-security.txt\n  keywords: [hackerone, responsible disclosure, security@mollie.com]\nprobes:\n- url: https://trust.mollie.com\n\
  \  status: 000\n  result: does not resolve\n- url: https://www.mollie.com/trust\n  status: 404\n- url: https://www.mollie.com/compliance\n  status: 404\n- url: https://www.mollie.com/security\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/security/mollie-trust-center.yml
summary_line: SOC 2 Type 2, PCI-DSS Level 1, ISAE 3402 Type 2, GDPR
tags:
- Company
- Payments
- Fintech
- Financial-Services
- Checkout
- E-Commerce
- Subscription
- Point-of-Sale
- Europe
- Netherlands
trust_url: https://www.mollie.com/security
---
