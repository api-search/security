---
api_specs:
- filename: pinch-payments-core.yml
  format: yaml
  label: Pinch Core API
  slug: pinch-payments-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-core.yml
- filename: pinch-payments-payments.yml
  format: yaml
  label: Pinch Payments API
  slug: pinch-payments-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payments.yml
- filename: pinch-payments-payers.yml
  format: yaml
  label: Pinch Payers API
  slug: pinch-payments-payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payers.yml
- filename: pinch-payments-payment-links.yml
  format: yaml
  label: Pinch Payment Links API
  slug: pinch-payments-payment-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payment-links.yml
- filename: pinch-payments-merchants.yml
  format: yaml
  label: Pinch Merchants API
  slug: pinch-payments-merchants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchants.yml
- filename: pinch-payments-webhooks.yml
  format: yaml
  label: Pinch Webhooks API
  slug: pinch-payments-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-webhooks.yml
- filename: pinch-payments-contacts.yml
  format: yaml
  label: Pinch Contacts API
  slug: pinch-payments-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-contacts.yml
- filename: pinch-payments-transfers.yml
  format: yaml
  label: Pinch Transfers API
  slug: pinch-payments-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-transfers.yml
- filename: pinch-payments-merchant-financial-data.yml
  format: yaml
  label: Pinch Merchant Financial Data API
  slug: pinch-payments-merchant-financial-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchant-financial-data.yml
- filename: pinch-payments-authentication.yml
  format: yaml
  label: Pinch Authentication API
  slug: pinch-payments-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-authentication.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getpinch.com.au
  spf: true
hosts:
- cert_expires: Sep  1 03:32:56 2026 GMT
  host: getpinch.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:29:05 2026 GMT
  host: docs.getpinch.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.getpinch.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinch Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinch Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pinch Payments
provider_slug: pinch-payments
slug: pinch-payments-domain-security
source_filename: pinch-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getpinch.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:32:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getpinch.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:29:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getpinch.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getpinch.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/security/pinch-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Direct Debit
- Card Payments
- Subscription
- Billing
- Payment Facilitator
- Account-to-Account
- New Zealand
---
