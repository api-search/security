---
api_specs:
- filename: stryke-api.yaml
  format: yaml
  label: Dopex CLAMM Options Trading API
  slug: clamm-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopex/refs/heads/main/openapi/stryke-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stryke.xyz
  spf: true
hosts:
- cert_expires: Aug 27 17:59:28 2026 GMT
  host: www.stryke.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 13:43:24 2026 GMT
  host: docs.stryke.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:06:43 2026 GMT
  host: api.stryke.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dopex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dopex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dopex
provider_slug: dopex
slug: dopex-domain-security
source_filename: dopex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stryke.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:59:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.stryke.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:43:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stryke.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:06:43 2026 GMT\n  hsts: null\ndomains:\n- domain: stryke.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopex/refs/heads/main/security/dopex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Decentralized Options
- SSOV
- Options Exchange
- Arbitrum
- DPX
- rDPX
- Staking
- Implied Volatility
- Black-Scholes
- Options Pricing
- CLAMM
- Cryptocurrency
- Web3
- EVM
---
