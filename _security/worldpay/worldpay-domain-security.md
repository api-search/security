---
api_specs:
- filename: openapi
  format: yaml
  label: Worldpay Card Payments API
  slug: worldpay-card-payments-api
  spec_type: OpenAPI
  url: https://docs.worldpay.com/access/products/payments/openapi
- filename: openapi
  format: yaml
  label: Worldpay Payment Queries API
  slug: worldpay-payment-queries-api
  spec_type: OpenAPI
  url: https://developer.worldpay.com/products/access/payment-queries/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: worldpay.com
  spf: true
hosts:
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: docs.worldpay.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: access.worldpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: try.access.worldpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worldpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worldpay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Worldpay
provider_slug: worldpay
slug: worldpay-domain-security
source_filename: worldpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.worldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: access.worldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: try.access.worldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: worldpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldpay/refs/heads/main/security/worldpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Payment Gateway
- Tokenization
- Fraud Prevention
- Recurring Billing
- Payouts
- Foreign Exchange
- Financial Services
- Fintech
---
