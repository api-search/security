---
api_specs:
- filename: openapi.json
  format: json
  label: MyStars FaaS Fulfilment API
  slug: mystars-faas-fulfilment-api
  spec_type: OpenAPI
  url: https://mystars.tg/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mystars.tg
  spf: true
hosts:
- cert_expires: Oct 13 03:25:59 2026 GMT
  host: mystars.tg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 03:25:59 2026 GMT
  host: api.mystars.tg
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Mystars Faas Fulfilment Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyStars FaaS — Fulfilment API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyStars FaaS — Fulfilment API
provider_slug: mystars-faas-fulfilment-api
slug: mystars-faas-fulfilment-api-domain-security
source_filename: mystars-faas-fulfilment-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mystars.tg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mystars.tg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:25:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mystars.tg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystars-faas-fulfilment-api/refs/heads/main/security/mystars-faas-fulfilment-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Telegram
- telegram-stars
- telegram-premium
- Payments
- Crypto
- TON
- gram
- USDT
- Fintech
- fulfilment
- Digital Goods
- Non-Custodial
- no-kyc
---
