---
api_specs:
- filename: raydium-openapi.yml
  format: yaml
  label: Raydium REST API v3
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raydium/refs/heads/main/openapi/raydium-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raydium.io
  spf: true
hosts:
- cert_expires: Sep 15 14:43:31 2026 GMT
  host: raydium.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:12:03 2026 GMT
  host: api-v3.raydium.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 11:49:08 2026 GMT
  host: docs.raydium.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raydium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raydium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Raydium
provider_slug: raydium
slug: raydium-domain-security
source_filename: raydium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raydium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:43:31 2026 GMT\n  hsts: false\n- host: api-v3.raydium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:12:03 2026 GMT\n  hsts: false\n- host: docs.raydium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:49:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: raydium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raydium/refs/heads/main/security/raydium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Solana
- DEX
- AMM
- Liquidity
- CLMM
- Launchpad
- Open Source
---
