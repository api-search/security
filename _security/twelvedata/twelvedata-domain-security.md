---
api_specs:
- filename: twelvedata-asyncapi.yml
  format: yaml
  label: Twelve Data WebSocket Streaming API
  slug: twelvedata-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/asyncapi/twelvedata-asyncapi.yml
- filename: twelvedata-core-data-api-openapi.yml
  format: yaml
  label: Twelve Data Core Data API
  slug: twelvedata-core-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-core-data-api-openapi.yml
- filename: twelvedata-fundamentals-api-openapi.yml
  format: yaml
  label: Twelve Data Fundamentals API
  slug: twelvedata-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-fundamentals-api-openapi.yml
- filename: twelvedata-reference-data-api-openapi.yml
  format: yaml
  label: Twelve Data Reference Data API
  slug: twelvedata-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-reference-data-api-openapi.yml
- filename: twelvedata-technical-indicators-api-openapi.yml
  format: yaml
  label: Twelve Data Technical Indicators API
  slug: twelvedata-technical-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-technical-indicators-api-openapi.yml
- filename: twelvedata-time-series-api-openapi.yml
  format: yaml
  label: Twelve Data Time Series API
  slug: twelvedata-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-time-series-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: twelvedata.com
  spf: true
hosts:
- cert_expires: Oct  8 06:43:27 2026 GMT
  host: twelvedata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:43:27 2026 GMT
  host: ws.twelvedata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:43:27 2026 GMT
  host: api.twelvedata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twelvedata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twelve Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Twelve Data
provider_slug: twelvedata
slug: twelvedata-domain-security
source_filename: twelvedata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twelvedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:43:27 2026 GMT\n  hsts: false\n- host: ws.twelvedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:43:27 2026 GMT\n  hsts: null\n- host: api.twelvedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:43:27 2026 GMT\n  hsts: null\ndomains:\n- domain: twelvedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/security/twelvedata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Market Data
- Financial Data
- Stocks
- Forex
- Crypto
- Real-Time Data
- Technical Indicators
- Fundamentals
---
