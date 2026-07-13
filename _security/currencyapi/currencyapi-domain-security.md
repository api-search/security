---
api_specs:
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Latest Exchange Rates API
  slug: currencyapi-latest-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Historical Exchange Rates API
  slug: currencyapi-historical-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Range Exchange Rates API
  slug: currencyapi-range-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Convert API
  slug: currencyapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Currencies API
  slug: currencyapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Status API
  slug: currencyapi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: currencyapi.com
  spf: true
hosts:
- cert_expires: Aug 22 06:54:35 2026 GMT
  host: currencyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 06:54:35 2026 GMT
  host: api.currencyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Currencyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CurrencyAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CurrencyAPI
provider_slug: currencyapi
slug: currencyapi-domain-security
source_filename: currencyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currencyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:54:35 2026 GMT\n  hsts: false\n- host: api.currencyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:54:35 2026 GMT\n  hsts: null\ndomains:\n- domain: currencyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/security/currencyapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Financial Data
---
