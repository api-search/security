---
api_specs:
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Indicators API
  slug: tradingeconomics-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Economic Calendar API
  slug: tradingeconomics-economic-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Markets API
  slug: tradingeconomics-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Forecasts API
  slug: tradingeconomics-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Historical API
  slug: tradingeconomics-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Financials API
  slug: tradingeconomics-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-asyncapi.yml
  format: yaml
  label: Trading Economics Streaming API
  slug: tradingeconomics-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/asyncapi/tradingeconomics-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tradingeconomics.com
  spf: false
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: tradingeconomics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:47:19 2026 GMT
  host: docs.tradingeconomics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.tradingeconomics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tradingeconomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trading Economics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Trading Economics
provider_slug: tradingeconomics
slug: tradingeconomics-domain-security
source_filename: tradingeconomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradingeconomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: docs.tradingeconomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:47:19 2026 GMT\n  hsts: false\n- host: api.tradingeconomics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tradingeconomics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/security/tradingeconomics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Economic Indicators
- Interest Rates
- Macroeconomics
- Financial Data
- Economic Calendar
- Forecasts
- Markets
---
