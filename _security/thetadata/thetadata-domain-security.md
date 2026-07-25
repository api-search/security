---
api_specs:
- filename: thetadata-streaming-asyncapi.yml
  format: yaml
  label: ThetaData Streaming WebSocket API
  slug: thetadata-streaming-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/asyncapi/thetadata-streaming-asyncapi.yml
- filename: thetadata-at-time-api-openapi.yml
  format: yaml
  label: ThetaData At-Time API
  slug: thetadata-at-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-at-time-api-openapi.yml
- filename: thetadata-calendar-api-openapi.yml
  format: yaml
  label: ThetaData Calendar API
  slug: thetadata-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-calendar-api-openapi.yml
- filename: thetadata-flatfile-api-openapi.yml
  format: yaml
  label: ThetaData FlatFile API
  slug: thetadata-flatfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-flatfile-api-openapi.yml
- filename: thetadata-history-api-openapi.yml
  format: yaml
  label: ThetaData History API
  slug: thetadata-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-history-api-openapi.yml
- filename: thetadata-index-api-openapi.yml
  format: yaml
  label: ThetaData Index API
  slug: thetadata-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-index-api-openapi.yml
- filename: thetadata-interest-rate-api-openapi.yml
  format: yaml
  label: ThetaData Interest Rate API
  slug: thetadata-interest-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-interest-rate-api-openapi.yml
- filename: thetadata-list-api-openapi.yml
  format: yaml
  label: ThetaData List API
  slug: thetadata-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-list-api-openapi.yml
- filename: thetadata-option-api-openapi.yml
  format: yaml
  label: ThetaData Option API
  slug: thetadata-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-option-api-openapi.yml
- filename: thetadata-single-day-api-openapi.yml
  format: yaml
  label: ThetaData Single Day API
  slug: thetadata-single-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-single-day-api-openapi.yml
- filename: thetadata-snapshot-api-openapi.yml
  format: yaml
  label: ThetaData Snapshot API
  slug: thetadata-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-snapshot-api-openapi.yml
- filename: thetadata-stock-api-openapi.yml
  format: yaml
  label: ThetaData Stock API
  slug: thetadata-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-stock-api-openapi.yml
- filename: thetadata-year-api-openapi.yml
  format: yaml
  label: ThetaData Year API
  slug: thetadata-year-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-year-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetadata.net
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: thetadata.us
  spf: false
hosts:
- cert_expires: Sep 24 13:54:04 2026 GMT
  host: thetadata.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 14:31:18 2026 GMT
  host: docs.thetadata.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Thetadata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThetaData, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThetaData
provider_slug: thetadata
slug: thetadata-domain-security
source_filename: thetadata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetadata.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:54:04 2026 GMT\n  hsts: false\n- host: docs.thetadata.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 14:31:18 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: thetadata.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: thetadata.us\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/security/thetadata-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Options
- Stocks
- Indices
- Real-Time
- Historical Data
- Trading
---
