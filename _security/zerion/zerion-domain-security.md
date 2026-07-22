---
api_specs:
- filename: zerion-openapi-original.yml
  format: yaml
  label: Zerion API
  slug: zerion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zerion.io
  spf: true
hosts:
- cert_expires: Oct  3 14:49:57 2026 GMT
  host: developers.zerion.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:57:44 2026 GMT
  host: api.zerion.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zerion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zerion
provider_slug: zerion
slug: zerion-domain-security
source_filename: zerion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.zerion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zerion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:57:44 2026 GMT\n  hsts: null\ndomains:\n- domain: zerion.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/security/zerion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Blockchain
- Cryptocurrency
- DeFi
- Wallet
- NFT
- Ethereum
- Solana
- Portfolio
- Onchain Data
- Transactions
---
