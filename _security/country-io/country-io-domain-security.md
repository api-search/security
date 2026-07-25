---
api_specs:
- filename: country-io-capitals-api-openapi.yml
  format: yaml
  label: Country.io Capitals API
  slug: country-io-capitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-capitals-api-openapi.yml
- filename: country-io-continents-api-openapi.yml
  format: yaml
  label: Country.io Continents API
  slug: country-io-continents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-continents-api-openapi.yml
- filename: country-io-currency-api-openapi.yml
  format: yaml
  label: Country.io Currency API
  slug: country-io-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-currency-api-openapi.yml
- filename: country-io-iso3-api-openapi.yml
  format: yaml
  label: Country.io ISO3 API
  slug: country-io-iso3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-iso3-api-openapi.yml
- filename: country-io-names-api-openapi.yml
  format: yaml
  label: Country.io Names API
  slug: country-io-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-names-api-openapi.yml
- filename: country-io-phone-api-openapi.yml
  format: yaml
  label: Country.io Phone API
  slug: country-io-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-phone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: country.io
  spf: false
hosts:
- cert_expires: Sep  9 18:51:21 2026 GMT
  host: country.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Country Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Country.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Country.io
provider_slug: country-io
slug: country-io-domain-security
source_filename: country-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: country.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:51:21 2026 GMT\n  hsts: false\ndomains:\n- domain: country.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/security/country-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Capitals
- Continents
- Countries
- Currencies
- Currency Codes
- Dialing Codes
- Geography
- ISO 3166
- JSON
- Open Data
- Phone Codes
- Reference Data
---
