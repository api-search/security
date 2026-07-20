---
api_specs:
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Checkout API
  slug: doku-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Access Token API
  slug: doku-snap-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Virtual Account API
  slug: doku-snap-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Direct Debit & e-Wallet API
  slug: doku-snap-direct-debit-ewallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP QRIS API
  slug: doku-snap-qris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Kirim Payout API
  slug: doku-kirim-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doku.com
  spf: true
  spf_record: v=spf1 include:spfdm-ap-southeast-1.aliyun.com ip4:103.10.128.0/22 include:spf.mandrillapp.com include:44284973.spf01.hubspotemail.net include:servers.mcsv.net include:ncapp02.com include:_spf.google.com ~all
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.doku.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:01:28 2026 GMT
  host: developers.doku.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.doku.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: api-sandbox.doku.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DOKU, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DOKU
provider_slug: doku
slug: doku-domain-security
source_filename: doku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: developers.doku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:01:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.doku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api-sandbox.doku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: doku.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spfdm-ap-southeast-1.aliyun.com ip4:103.10.128.0/22 include:spf.mandrillapp.com include:44284973.spf01.hubspotemail.net include:servers.mcsv.net\
  \ include:ncapp02.com include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\nnotes: >-\n  All API and developer hosts serve TLS 1.3 with HSTS; the production API host\n  (api.doku.com) additionally sets includeSubDomains and preload. No CAA record\n  is published on doku.com and DNSSEC is not enabled. DMARC policy is quarantine\n  (not reject). Region hosting is Asia Pacific (SE Asia / Indonesia), consistent\n  with the aliyun ap-southeast-1 SPF include.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/security/doku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Fintech
- Indonesia
- SEA
- SNAP
- Virtual Account
- E-Wallet
- QRIS
- Direct Debit
- Payouts
---
