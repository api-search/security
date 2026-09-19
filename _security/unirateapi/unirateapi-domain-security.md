---
api_specs:
- filename: unirateapi-commodity-api-openapi.yml
  format: yaml
  label: UniRate API Commodity API
  slug: unirateapi-commodity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-commodity-api-openapi.yml
- filename: unirateapi-currency-api-openapi.yml
  format: yaml
  label: UniRate API Currency API
  slug: unirateapi-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-currency-api-openapi.yml
- filename: unirateapi-historical-currency-api-openapi.yml
  format: yaml
  label: UniRate API Historical Currency API
  slug: unirateapi-historical-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-historical-currency-api-openapi.yml
- filename: unirateapi-vat-rates-api-openapi.yml
  format: yaml
  label: UniRate API VAT Rates API
  slug: unirateapi-vat-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-vat-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unirateapi.com
  spf: true
hosts:
- cert_expires: Oct 29 05:28:46 2026 GMT
  host: unirateapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 05:28:46 2026 GMT
  host: api.unirateapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Unirateapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniRate API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UniRate API
provider_slug: unirateapi
slug: unirateapi-domain-security
source_filename: unirateapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unirateapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 05:28:46 2026 GMT\n  hsts: false\n- host: api.unirateapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 05:28:46 2026 GMT\n  hsts: false\ndomains:\n- domain: unirateapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/security/unirateapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency
- Exchange Rates
- Foreign Exchange
- Forex
- Currency Conversion
- VAT
- Finance
- Financial Data
---
