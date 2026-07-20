---
api_specs:
- filename: brl-openapi-original.json
  format: json
  label: Crown API & Webhooks
  slug: crown-api-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brl/refs/heads/main/openapi/brl-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brl.xyz
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crown-brlv.com
  spf: true
hosts:
- cert_expires: Sep  7 11:15:07 2026 GMT
  host: brl.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 01:52:24 2026 GMT
  host: docs.crown-brlv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: app.crown-brlv.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BRL
provider_slug: brl
slug: brl-domain-security
source_filename: brl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brl.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:15:07 2026 GMT\n  hsts: false\n- host: docs.crown-brlv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.crown-brlv.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: brl.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: crown-brlv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brl/refs/heads/main/security/brl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Stablecoin
- Payments
- Brazil
- PIX
- Fintech
- Blockchain
- Digital Assets
- Wallets
- Yield
---
