---
api_specs:
- filename: openapi.yml
  format: yaml
  label: PayFast Payments API
  slug: payfast-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payfast.io
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:technical@payfast.co.za"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payfast.co.za
  spf: true
hosts:
- cert_expires: Sep 14 07:29:29 2026 GMT
  host: payfast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.payfast.co.za
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.payfast.co.za
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payfast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayFast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PayFast
provider_slug: payfast
slug: payfast-domain-security
source_filename: payfast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payfast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:29:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.payfast.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.payfast.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: payfast.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: payfast.co.za\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:technical@payfast.co.za\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/security/payfast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- South Africa
- Subscriptions
- Recurring Billing
- Tokenization
- Instant EFT
- QR Code Payments
- Refunds
- Fintech
---
