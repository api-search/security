---
api_specs:
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Filing Query API
  slug: sec-api-filing-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Full-Text Search API
  slug: sec-api-full-text-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-asyncapi.yml
  format: yaml
  label: SEC API Filing Stream API
  slug: sec-api-filing-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/asyncapi/sec-api-asyncapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API XBRL-to-JSON Converter API
  slug: sec-api-xbrl-to-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Extractor API
  slug: sec-api-extractor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Insider Trading API
  slug: sec-api-insider-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Form 13F Holdings API
  slug: sec-api-form-13f-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sec-api.io
  spf: false
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: sec-api.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.sec-api.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: stream.sec-api.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sec Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEC API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SEC API
provider_slug: sec-api
slug: sec-api-domain-security
source_filename: sec-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI + WebSocket hosts\nhosts:\n- host: sec-api.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.sec-api.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: stream.sec-api.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sec-api.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/security/sec-api-domain-security.yml
summary_line: TLSv1.3
tags:
- SEC Filings
- Regulatory Filings
- EDGAR
- Financial Data
- Compliance
- Government Reports
- Insider Trading
- 13F
- XBRL
- Full-Text Search
---
