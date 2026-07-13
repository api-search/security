---
api_specs:
- filename: currencybeacon-openapi.yml
  format: yaml
  label: CurrencyBeacon API
  slug: currencybeacon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencybeacon/refs/heads/main/openapi/currencybeacon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: currencybeacon.com
  spf: true
hosts:
- cert_expires: Sep  1 00:34:45 2026 GMT
  host: currencybeacon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:34:45 2026 GMT
  host: api.currencybeacon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Currencybeacon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CurrencyBeacon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CurrencyBeacon
provider_slug: currencybeacon
slug: currencybeacon-domain-security
source_filename: currencybeacon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currencybeacon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:34:45 2026 GMT\n  hsts: false\n- host: api.currencybeacon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:34:45 2026 GMT\n  hsts: false\ndomains:\n- domain: currencybeacon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencybeacon/refs/heads/main/security/currencybeacon-domain-security.yml
summary_line: TLSv1.3
tags:
- Currency
- Exchange Rates
- Forex
- Cryptocurrency
- Financial Data
- Historical Rates
- Currency Conversion
---
