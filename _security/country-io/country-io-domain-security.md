---
api_specs:
- filename: country-io-data-openapi.yml
  format: yaml
  label: Country.io Data API
  slug: country-io-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-io/refs/heads/main/openapi/country-io-data-openapi.yml
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
