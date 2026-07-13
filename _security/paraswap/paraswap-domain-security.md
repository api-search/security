---
api_specs:
- filename: ae3be6da4dbc8376e17f526f04ada75d
  format: yaml
  label: ParaSwap Market API
  slug: paraswap-market-api
  spec_type: OpenAPI
  url: https://gist.github.com/SpotLabsNET/ae3be6da4dbc8376e17f526f04ada75d
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: velora.xyz
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paraswap.io
  spf: true
hosts:
- cert_expires: Oct  8 22:11:36 2026 GMT
  host: www.velora.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: developers.velora.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.paraswap.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paraswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParaSwap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ParaSwap
provider_slug: paraswap
slug: paraswap-domain-security
source_filename: paraswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.velora.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.velora.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paraswap.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: velora.xyz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: paraswap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paraswap/refs/heads/main/security/paraswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- DEX Aggregator
- Token Swaps
- Blockchain
- EVM
- Cryptocurrency
- Liquidity
- Smart Contracts
---
