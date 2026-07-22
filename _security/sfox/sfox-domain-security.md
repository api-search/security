---
api_specs:
- filename: rest-endpoints
  format: yaml
  label: sFOX REST API
  slug: sfox-rest-api
  spec_type: OpenAPI
  url: https://docs.sfox.com/rest-api/rest-endpoints
- filename: sfox-websocket-asyncapi.yml
  format: yaml
  label: sFOX WebSocket API
  slug: sfox-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfox/refs/heads/main/asyncapi/sfox-websocket-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sfox.com
  spf: true
hosts:
- cert_expires: Sep  2 08:31:12 2026 GMT
  host: docs.sfox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 15:46:35 2026 GMT
  host: api.sfox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:10:18 2026 GMT
  host: ws.sfox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sfox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sfox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sfox
provider_slug: sfox
slug: sfox-domain-security
source_filename: sfox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:46:35 2026 GMT\n  hsts: null\n- host: ws.sfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:10:18 2026 GMT\n  hsts: null\ndomains:\n- domain: sfox.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sfox/refs/heads/main/security/sfox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Prime Brokerage
- Trading
- Digital Asset Custody
- Liquidity
- Staking
- Institutional
- Financial Services
- Market Data
- WebSocket
- FIX
---
