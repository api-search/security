---
api_specs:
- filename: blue-square-group-limited-streams.yml
  format: yaml
  label: GRVT Market Data API
  slug: grvt-market-data-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-square-group-limited/refs/heads/main/asyncapi/blue-square-group-limited-streams.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grvt.io
  spf: true
hosts:
- cert_expires: Sep 24 17:46:46 2026 GMT
  host: grvt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:46:46 2026 GMT
  host: api-docs.grvt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:46:46 2026 GMT
  host: market-data.grvt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blue Square Group Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Square Group Limited, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blue Square Group Limited
provider_slug: blue-square-group-limited
slug: blue-square-group-limited-domain-security
source_filename: blue-square-group-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grvt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.grvt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:46:46 2026 GMT\n  hsts: false\n- host: market-data.grvt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:46:46 2026 GMT\n  hsts: null\ndomains:\n- domain: grvt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-square-group-limited/refs/heads/main/security/blue-square-group-limited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Derivatives Exchange
- Trading
- Perpetual Futures
- Market Data
- Blockchain
- WebSocket
- Financial Services
---
