---
api_specs:
- filename: koin-payments-openapi.json
  format: json
  label: Koin Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payments-openapi.json
- filename: koin-antifraud-evaluations-openapi.json
  format: json
  label: Koin Antifraud API
  slug: antifraud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-antifraud-evaluations-openapi.json
- filename: koin-onboarding-openapi.json
  format: json
  label: Koin Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-onboarding-openapi.json
- filename: koin-bnpl-openapi.json
  format: json
  label: Koin BNPL Payment Request API
  slug: bnpl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-bnpl-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: koin.com.br
  spf: true
hosts:
- cert_expires: Aug 30 03:15:24 2026 GMT
  host: www.koin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:19:04 2026 GMT
  host: api-docs.koin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api-sandbox.koin.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koin
provider_slug: koin
slug: koin-domain-security
source_filename: koin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:19:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: koin.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/security/koin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fraud Prevention
- Buy Now Pay Later
- Pix
- E-Commerce
- Financial Services
- Brazil
- Latin America
- Anti-Fraud
- Checkout
- Company
---
