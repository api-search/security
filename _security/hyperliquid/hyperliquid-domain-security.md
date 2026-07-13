---
api_specs:
- filename: hyperliquid-asyncapi.yml
  format: yaml
  label: Hyperliquid WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperliquid/refs/heads/main/asyncapi/hyperliquid-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hyperliquid.xyz
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: hyperliquid.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: hyperliquid.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.hyperliquid.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperliquid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperliquid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Hyperliquid
provider_slug: hyperliquid
slug: hyperliquid-domain-security
source_filename: hyperliquid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperliquid.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: hyperliquid.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hyperliquid.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hyperliquid.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperliquid/refs/heads/main/security/hyperliquid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Perpetuals
- DEX
- Layer 1
- Trading
- Order Book
- HyperEVM
---
