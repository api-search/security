---
api_specs:
- filename: openapi.yml
  format: yaml
  label: PancakeSwap Info API v2
  slug: pancakeswap-info-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/openapi/openapi.yml
- filename: profile-openapi.yml
  format: yaml
  label: PancakeSwap Profile API
  slug: pancakeswap-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/openapi/profile-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pancakeswap.finance
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pancakeswap.info
  spf: true
hosts:
- cert_expires: Sep 17 23:02:57 2026 GMT
  host: pancakeswap.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:59:37 2026 GMT
  host: api.pancakeswap.info
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: nodereal.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pancakeswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PancakeSwap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PancakeSwap
provider_slug: pancakeswap
slug: pancakeswap-domain-security
source_filename: pancakeswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pancakeswap.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:02:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pancakeswap.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:59:37 2026 GMT\n  hsts: null\n- host: nodereal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pancakeswap.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pancakeswap.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/security/pancakeswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- DEX
- BNB Chain
- Decentralized Exchange
- Blockchain
- Swap
- Liquidity
- Yield Farming
- NFT
- Web3
---
