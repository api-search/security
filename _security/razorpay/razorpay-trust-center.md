---
api_specs:
- filename: razorpay-openapi.yml
  format: yaml
  label: Razorpay Core REST API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/openapi/razorpay-openapi.yml
- filename: razorpay-webhooks-asyncapi.yml
  format: yaml
  label: Razorpay Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/asyncapi/razorpay-webhooks-asyncapi.yml
certifications:
- PCI DSS
- ISO 27001
- SOC 2
description: Razorpay's security & compliance posture, captured from razorpay.com/docs/security and the published PCI DSS certificate. Razorpay is a PCI-DSS certified payment service provider handling cardholder data, with its cardholder data environment assessed by an external QSA (Ampcus Cyber). Compliance program covers PCI-DSS, ISO 27001, and SOC 2. Certificate copies are provided on request via a Key Account Manager, so the automated trust-center probe (which requires a trust.<domain> subdomain and keyword threshold) does not record it — this is the searched, human-verified fill.
kind: trust-center
layout: security
name: Razorpay Trust Center
name_suffix: Trust Center
overview: Razorpay maintains a public trust center documenting PCI DSS, ISO 27001, and SOC 2 compliance.
provider_name: Razorpay
provider_slug: razorpay
slug: razorpay-trust-center
source_filename: razorpay-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://razorpay.com/docs/security/\nurl: https://razorpay.com/docs/security/\ndescription: >-\n  Razorpay's security & compliance posture, captured from razorpay.com/docs/security\n  and the published PCI DSS certificate. Razorpay is a PCI-DSS certified payment\n  service provider handling cardholder data, with its cardholder data environment\n  assessed by an external QSA (Ampcus Cyber). Compliance program covers PCI-DSS,\n  ISO 27001, and SOC 2. Certificate copies are provided on request via a Key\n  Account Manager, so the automated trust-center probe (which requires a\n  trust.<domain> subdomain and keyword threshold) does not record it — this is\n  the searched, human-verified fill.\ncertifications:\n  - {name: PCI DSS, scope: Payment service provider — cardholder data environment, assessor: Ampcus Cyber Inc. (QSA), note: Certificate published; copies available on request.}\n  - {name: ISO 27001, note: Information\
  \ security management system compliance.}\n  - {name: SOC 2, note: Part of Razorpay's stated global compliance program.}\ndata_protection:\n  transport: HTTPS/TLS with industry-standard ciphers; EV SSL certificate.\n  encryption_at_rest: AES-128-bit encryption for user data.\n  pii: Field-level encryption for personally identifiable information.\nreport_access:\n  method: Certification copies provided on request via a Key Account Manager.\ndocs:\n  - https://razorpay.com/docs/security/\n  - https://razorpay.com/docs/security/shared-responsibility-model/\n  - https://razorpay.com/docs/build/browser/assets/images/pci-dss-us.pdf\nevidence:\n  - {source: https://razorpay.com/docs/security/, keywords: [pci-dss, tls, aes-128, ev ssl, field-level encryption]}\n  - {source: https://www.ampcuscyber.com/certificate/razorpay-pci-dss-coc.pdf, kind: pci-dss-certificate}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/security/razorpay-trust-center.yml
summary_line: PCI DSS, ISO 27001, SOC 2
tags:
- Payments
- Payment Gateway
- Fintech
- India
- UPI
- Subscriptions
- Payouts
- Checkout
trust_url: https://razorpay.com/docs/security/
---
