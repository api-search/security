---
api_specs:
- filename: open-exchange-rates-convert-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Convert API
  slug: open-exchange-rates-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-convert-api-openapi.yml
- filename: open-exchange-rates-currencies-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Currencies API
  slug: open-exchange-rates-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-currencies-api-openapi.yml
- filename: open-exchange-rates-ohlc-api-openapi.yml
  format: yaml
  label: Open Exchange Rates OHLC API
  slug: open-exchange-rates-ohlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-ohlc-api-openapi.yml
- filename: open-exchange-rates-rates-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Rates API
  slug: open-exchange-rates-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-rates-api-openapi.yml
- filename: open-exchange-rates-time-series-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Time Series API
  slug: open-exchange-rates-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-time-series-api-openapi.yml
- filename: open-exchange-rates-usage-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Usage API
  slug: open-exchange-rates-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openexchangerates.org
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: openexchangerates.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Exchange Rates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Exchange Rates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open Exchange Rates
provider_slug: open-exchange-rates
slug: open-exchange-rates-domain-security
source_filename: open-exchange-rates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openexchangerates.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: openexchangerates.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/security/open-exchange-rates-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Foreign Exchange
- Currency
- Forex
- Finance
- Exchange Rates
- Currency Conversion
- Historical Rates
---
