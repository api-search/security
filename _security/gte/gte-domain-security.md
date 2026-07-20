---
api_specs:
- filename: gte-openapi-original.yml
  format: yaml
  label: GTE API
  slug: gte-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/openapi/gte-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gte.xyz
  spf: false
hosts:
- cert_expires: Sep 12 15:02:59 2026 GMT
  host: www.gte.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api-testnet.gte.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GTE, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: GTE
provider_slug: gte
slug: gte-domain-security
source_filename: gte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gte.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:02:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-testnet.gte.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gte.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/security/gte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Defi
- Decentralized Exchange
- Trading
- Market Data
- Order Book
- Perpetuals
- MegaETH
- Blockchain
---
