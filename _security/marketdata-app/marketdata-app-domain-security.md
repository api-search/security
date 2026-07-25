---
api_specs:
- filename: marketdata-app-indices-api-openapi.yml
  format: yaml
  label: Market Data Indices API
  slug: marketdata-app-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-indices-api-openapi.yml
- filename: marketdata-app-markets-api-openapi.yml
  format: yaml
  label: Market Data Markets API
  slug: marketdata-app-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-markets-api-openapi.yml
- filename: marketdata-app-options-api-openapi.yml
  format: yaml
  label: Market Data Options API
  slug: marketdata-app-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-options-api-openapi.yml
- filename: marketdata-app-stocks-api-openapi.yml
  format: yaml
  label: Market Data Stocks API
  slug: marketdata-app-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-stocks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marketdata.app
  spf: true
hosts:
- cert_expires: Oct 20 18:45:55 2026 GMT
  host: www.marketdata.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 18:45:55 2026 GMT
  host: api.marketdata.app
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketdata App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Market Data, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Market Data
provider_slug: marketdata-app
slug: marketdata-app-domain-security
source_filename: marketdata-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketdata.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 18:45:55 2026 GMT\n  hsts: false\n- host: api.marketdata.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 18:45:55 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: marketdata.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/security/marketdata-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Market Data
- Financial Data
- Stocks
- Options
- Indices
- Real-Time Data
- Historical Data
- Quotes
---
