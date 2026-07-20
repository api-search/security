---
api_specs:
- filename: bullet-trading-api-openapi.json
  format: json
  label: Bullet Trading API
  slug: bullet-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bullet/refs/heads/main/openapi/bullet-trading-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bullet.xyz
  spf: true
hosts:
- cert_expires: Oct  5 16:06:21 2026 GMT
  host: www.bullet.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 12:21:55 2026 GMT
  host: tradingapi.mainnet.bullet.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:30:39 2026 GMT
  host: tradingapi.testnet.bullet.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bullet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bullet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bullet
provider_slug: bullet
slug: bullet-domain-security
source_filename: bullet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bullet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:06:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tradingapi.mainnet.bullet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:21:55 2026 GMT\n  hsts: false\n- host: tradingapi.testnet.bullet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:30:39 2026 GMT\n  hsts: false\ndomains:\n- domain: bullet.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bullet/refs/heads/main/security/bullet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Solana
- Cryptocurrency
- Derivatives
- Exchange
- Trading
- Perpetuals
- Lending
- Blockchain
---
