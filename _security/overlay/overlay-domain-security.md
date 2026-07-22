---
api_specs:
- filename: overlay-openapi.yml
  format: yaml
  label: Overlay Market Data API
  slug: overlay-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overlay/refs/heads/main/openapi/overlay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: overlay.market
  spf: true
hosts:
- cert_expires: Aug 25 21:56:19 2026 GMT
  host: overlay.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 21:56:19 2026 GMT
  host: api.overlay.market
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overlay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overlay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Overlay
provider_slug: overlay
slug: overlay-domain-security
source_filename: overlay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: overlay.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:56:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.overlay.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:56:19 2026 GMT\n  hsts: null\ndomains:\n- domain: overlay.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overlay/refs/heads/main/security/overlay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defi
- DeFi
- Perpetual Futures
- Derivatives
- Trading
- Market Data
- BNB Smart Chain
- Blockchain
- Web3
---
