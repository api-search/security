---
api_specs:
- filename: infoway-real-time-market-data-api-streaming-asyncapi.yml
  format: yaml
  label: Infoway WebSocket Streaming API
  slug: infoway-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/asyncapi/infoway-real-time-market-data-api-streaming-asyncapi.yml
- filename: infoway-real-time-market-data-api-common-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Common API
  slug: infoway-real-time-market-data-api-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-common-api-openapi.yml
- filename: infoway-real-time-market-data-api-crypto-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Crypto API
  slug: infoway-real-time-market-data-api-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-crypto-api-openapi.yml
- filename: infoway-real-time-market-data-api-stock-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Stock API
  slug: infoway-real-time-market-data-api-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-stock-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infoway.io
  spf: true
hosts:
- cert_expires: Oct  9 15:28:21 2026 GMT
  host: docs.infoway.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:28:19 2026 GMT
  host: data.infoway.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infoway Real Time Market Data Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infoway Real-time Market Data API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infoway Real-time Market Data API
provider_slug: infoway-real-time-market-data-api
slug: infoway-real-time-market-data-api-domain-security
source_filename: infoway-real-time-market-data-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.infoway.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.infoway.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:28:19 2026 GMT\n  hsts: null\ndomains:\n- domain: infoway.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/security/infoway-real-time-market-data-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- stock-api
- forex-api
- crypto-api
- commodities-api
- futures-api
- market-data
- real-time-data
- websocket
- financial-data
- fintech
- historical-data
---
