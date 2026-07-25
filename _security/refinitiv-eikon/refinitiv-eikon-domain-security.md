---
api_specs:
- filename: refinitiv-eikon-asyncapi.yml
  format: yaml
  label: LSEG WebSocket API
  slug: lseg-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/asyncapi/refinitiv-eikon-asyncapi.yml
- filename: refinitiv-eikon-authentication-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Authentication API
  slug: refinitiv-eikon-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-authentication-api-openapi.yml
- filename: refinitiv-eikon-esg-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon ESG API
  slug: refinitiv-eikon-esg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-esg-api-openapi.yml
- filename: refinitiv-eikon-extractions-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Extractions API
  slug: refinitiv-eikon-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-extractions-api-openapi.yml
- filename: refinitiv-eikon-files-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Files API
  slug: refinitiv-eikon-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-files-api-openapi.yml
- filename: refinitiv-eikon-historical-pricing-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Historical Pricing API
  slug: refinitiv-eikon-historical-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-historical-pricing-api-openapi.yml
- filename: refinitiv-eikon-instrument-lists-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Instrument Lists API
  slug: refinitiv-eikon-instrument-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-instrument-lists-api-openapi.yml
- filename: refinitiv-eikon-jobs-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Jobs API
  slug: refinitiv-eikon-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-jobs-api-openapi.yml
- filename: refinitiv-eikon-news-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon News API
  slug: refinitiv-eikon-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-news-api-openapi.yml
- filename: refinitiv-eikon-on-demand-extractions-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon On-Demand Extractions API
  slug: refinitiv-eikon-on-demand-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-on-demand-extractions-api-openapi.yml
- filename: refinitiv-eikon-report-templates-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Report Templates API
  slug: refinitiv-eikon-report-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-report-templates-api-openapi.yml
- filename: refinitiv-eikon-schedules-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Schedules API
  slug: refinitiv-eikon-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-schedules-api-openapi.yml
- filename: refinitiv-eikon-search-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Search API
  slug: refinitiv-eikon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-search-api-openapi.yml
- filename: refinitiv-eikon-streaming-pricing-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Streaming Pricing API
  slug: refinitiv-eikon-streaming-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-streaming-pricing-api-openapi.yml
- filename: refinitiv-eikon-symbology-api-openapi.yml
  format: yaml
  label: Refinitiv Eikon Symbology API
  slug: refinitiv-eikon-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/openapi/refinitiv-eikon-symbology-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lseg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: refinitiv.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developers.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: www.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.refinitiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refinitiv Eikon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refinitiv Eikon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Refinitiv Eikon
provider_slug: refinitiv-eikon
slug: refinitiv-eikon-domain-security
source_filename: refinitiv-eikon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.refinitiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lseg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: refinitiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/security/refinitiv-eikon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Financial Data
- Financial News
- Market Data
- Real-Time Data
- Trading
---
