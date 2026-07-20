---
api_specs:
- filename: dodo-trade-openapi.yml
  format: yaml
  label: DODO Trade / Route API
  slug: dodo-trade-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo/refs/heads/main/openapi/dodo-trade-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dodoex.io
  spf: true
hosts:
- cert_expires: Sep 29 23:12:57 2026 GMT
  host: dodoex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DODO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DODO
provider_slug: dodo
slug: dodo-domain-security
source_filename: dodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dodoex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:12:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dodoex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dodo/refs/heads/main/security/dodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- DeFi
- DEX
- Decentralized Exchange
- Blockchain
- Trading
- Liquidity
- Web3
- Swap
---
