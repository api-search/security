---
api_specs:
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Latest Rates API
  slug: openexchangerates-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Historical Rates API
  slug: openexchangerates-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Time Series API
  slug: openexchangerates-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Convert API
  slug: openexchangerates-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Currencies API
  slug: openexchangerates-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates OHLC API
  slug: openexchangerates-ohlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Usage API
  slug: openexchangerates-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
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
- cert_expires: Oct  3 12:03:30 2026 GMT
  host: docs.openexchangerates.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openexchangerates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Exchange Rates, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open Exchange Rates
provider_slug: openexchangerates
slug: openexchangerates-domain-security
source_filename: openexchangerates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openexchangerates.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.openexchangerates.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openexchangerates.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/security/openexchangerates-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Forex
- Financial Data
---
