---
api_specs:
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
- filename: polygon-aggregates-api-openapi.yml
  format: yaml
  label: Polygon Aggregates API
  slug: polygon-aggregates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-aggregates-api-openapi.yml
- filename: polygon-books-api-openapi.yml
  format: yaml
  label: Polygon Books API
  slug: polygon-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-books-api-openapi.yml
- filename: polygon-contracts-api-openapi.yml
  format: yaml
  label: Polygon Contracts API
  slug: polygon-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-contracts-api-openapi.yml
- filename: polygon-conversion-api-openapi.yml
  format: yaml
  label: Polygon Conversion API
  slug: polygon-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-conversion-api-openapi.yml
- filename: polygon-corporateactions-api-openapi.yml
  format: yaml
  label: Polygon CorporateActions API
  slug: polygon-corporateactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-corporateactions-api-openapi.yml
- filename: polygon-dailybars-api-openapi.yml
  format: yaml
  label: Polygon DailyBars API
  slug: polygon-dailybars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-dailybars-api-openapi.yml
- filename: polygon-markets-api-openapi.yml
  format: yaml
  label: Polygon Markets API
  slug: polygon-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-markets-api-openapi.yml
- filename: polygon-news-api-openapi.yml
  format: yaml
  label: Polygon News API
  slug: polygon-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-news-api-openapi.yml
- filename: polygon-quotes-api-openapi.yml
  format: yaml
  label: Polygon Quotes API
  slug: polygon-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-quotes-api-openapi.yml
- filename: polygon-snapshots-api-openapi.yml
  format: yaml
  label: Polygon Snapshots API
  slug: polygon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-snapshots-api-openapi.yml
- filename: polygon-tickers-api-openapi.yml
  format: yaml
  label: Polygon Tickers API
  slug: polygon-tickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-tickers-api-openapi.yml
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
