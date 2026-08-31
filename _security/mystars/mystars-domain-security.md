---
api_specs:
- filename: mystars-mystars-faas-fulfilment-api-api-openapi.yml
  format: yaml
  label: MyStars FaaS MyStars FaaS — Fulfilment API
  slug: mystars-mystars-faas-fulfilment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-mystars-faas-fulfilment-api-api-openapi.yml
- filename: mystars-orders-api-openapi.yml
  format: yaml
  label: MyStars FaaS Orders API
  slug: mystars-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-orders-api-openapi.yml
- filename: mystars-pricing-api-openapi.yml
  format: yaml
  label: MyStars FaaS Pricing API
  slug: mystars-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-pricing-api-openapi.yml
- filename: mystars-recipients-api-openapi.yml
  format: yaml
  label: MyStars FaaS Recipients API
  slug: mystars-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-recipients-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Mystars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyStars FaaS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyStars FaaS
provider_slug: mystars
slug: mystars-domain-security
source_filename: mystars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mystars.tg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mystars.tg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:25:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mystars.tg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/security/mystars-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Telegram
- telegram-stars
- telegram-premium
- Payments
- Crypto
- TON
- Fulfilment
- Blockchain
- Digital Goods
- reseller-api
---
