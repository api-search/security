---
api_specs:
- filename: payu-europe-rest-api.yaml
  format: yaml
  label: PayU Europe REST API
  slug: payu-europe-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-europe-rest-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payu.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: corporate.payu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: developers.payu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: secure.payu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayU, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayU
provider_slug: payu
slug: payu-domain-security
source_filename: payu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: payu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/security/payu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Fintech
- Financial Services
- Subscriptions
- Fraud Detection
- Checkout
- Marketplace
- Tokenization
- Emerging Markets
---
