---
api_specs:
- filename: maverick-protocol-openapi.yaml
  format: yaml
  label: Maverick V2 Data API
  slug: maverick-v2-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maverick-protocol/refs/heads/main/openapi/maverick-protocol-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mav.xyz
  spf: true
hosts:
- cert_expires: Aug 26 22:08:09 2026 GMT
  host: www.mav.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maverick Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maverick Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maverick Protocol
provider_slug: maverick-protocol
slug: maverick-protocol-domain-security
source_filename: maverick-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mav.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:08:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mav.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maverick-protocol/refs/heads/main/security/maverick-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- DeFi
- DEX
- AMM
- Blockchain
- Market Data
- Liquidity
---
