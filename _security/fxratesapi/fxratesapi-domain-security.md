---
api_specs:
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Latest Rates API
  slug: fxratesapi-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Historical Rates API
  slug: fxratesapi-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Time-Series API
  slug: fxratesapi-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Convert API
  slug: fxratesapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Currencies API
  slug: fxratesapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fxratesapi.com
  spf: true
  spf_record: v=spf1 mx include:spf.w4ymail.at -all
hosts:
- cert_expires: Oct  7 10:36:56 2026 GMT
  host: api.fxratesapi.com
  hsts: null
  http_version: HTTP/2
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 13:54:49 2026 GMT
  host: fxratesapi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_version: HTTP/2
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fxratesapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FXRatesAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FXRatesAPI
provider_slug: fxratesapi
slug: fxratesapi-domain-security
source_filename: fxratesapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.fxratesapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:36:56 2026 GMT\n  hsts: null\n  http_version: HTTP/2\n- host: fxratesapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_version: HTTP/2\ndomains:\n- domain: fxratesapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 mx include:spf.w4ymail.at -all'\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  The API host api.fxratesapi.com serves HTTP/2 over TLS 1.3 but did not return\n  an HSTS header on the probed /latest response. The marketing host\n  fxratesapi.com returns HSTS (max-age 63072000, includeSubDomains, preload).\n  No CAA records are published for fxratesapi.com. DMARC is present but set to\n  p=none (monitor\
  \ only). SPF is published with a hard fail (-all).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/security/fxratesapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Foreign Exchange
- FX
- Currency
- Exchange Rates
- Forex
- Currency Conversion
- Historical Rates
- Financial Data
- Cryptocurrencies
---
