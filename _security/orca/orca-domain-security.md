---
api_specs:
- filename: orca-openapi-original.json
  format: json
  label: Orca Public API
  slug: orca-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orca/refs/heads/main/openapi/orca-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orca.so
  spf: true
hosts:
- cert_expires: Oct 17 18:56:14 2026 GMT
  host: orca.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orca
provider_slug: orca
slug: orca-domain-security
source_filename: orca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orca.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orca.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orca/refs/heads/main/security/orca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defi Dex
- DeFi
- DEX
- Solana
- AMM
- Liquidity
- Concentrated Liquidity
- Blockchain
- Crypto
---
