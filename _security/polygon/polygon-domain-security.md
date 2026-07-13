---
api_specs:
- filename: polygon-stocks-openapi.yml
  format: yaml
  label: Polygon Stocks API
  slug: stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-stocks-openapi.yml
- filename: polygon-options-openapi.yml
  format: yaml
  label: Polygon Options API
  slug: options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-options-openapi.yml
- filename: polygon-indices-openapi.yml
  format: yaml
  label: Polygon Indices API
  slug: indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-indices-openapi.yml
- filename: polygon-forex-openapi.yml
  format: yaml
  label: Polygon Forex API
  slug: forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-forex-openapi.yml
- filename: polygon-crypto-openapi.yml
  format: yaml
  label: Polygon Crypto API
  slug: crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-crypto-openapi.yml
- filename: polygon-reference-openapi.yml
  format: yaml
  label: Polygon Reference API
  slug: reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-reference-openapi.yml
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polygon.io
  spf: true
hosts:
- cert_expires: Sep 25 13:20:04 2026 GMT
  host: polygon.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 17:54:19 2026 GMT
  host: api.polygon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:51:56 2026 GMT
  host: socket.polygon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polygon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polygon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Polygon
provider_slug: polygon
slug: polygon-domain-security
source_filename: polygon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polygon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:20:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.polygon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 17:54:19 2026 GMT\n  hsts: null\n- host: socket.polygon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:51:56 2026 GMT\n  hsts: null\ndomains:\n- domain: polygon.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/security/polygon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Fintech
- Market Data
- Stocks
- Options
- Forex
- Crypto
- Indices
- Futures
- WebSockets
- Real-time
- Historical
- Public APIs
---
