---
api_specs:
- filename: monoova-payments.yml
  format: yaml
  label: Monoova Payments API
  slug: monoova-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-payments.yml
- filename: monoova-payto.yml
  format: yaml
  label: Monoova PayTo API
  slug: monoova-payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-payto.yml
- filename: monoova-cc.yml
  format: yaml
  label: Monoova Card Payments API
  slug: monoova-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-cc.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monoova.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mpay.com.au
  spf: true
hosts:
- cert_expires: Sep  9 02:10:02 2026 GMT
  host: www.monoova.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 13:22:57 2026 GMT
  host: developer.monoova.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:31:05 2026 GMT
  host: api.mpay.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Monoova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monoova, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monoova
provider_slug: monoova
slug: monoova-domain-security
source_filename: monoova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monoova.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.monoova.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mpay.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 01:31:05 2026 GMT\n  hsts: null\ndomains:\n- domain: monoova.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mpay.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/security/monoova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Real-Time Payments
- NPP
- PayTo
- PayID
- Account-to-Account
- BPAY
- Card Payments
- Money Movement
- Virtual Accounts
- Cross-Border
---
