---
api_specs:
- filename: country-state-city-api-openapi.yml
  format: yaml
  label: Country State City API
  slug: country-state-city-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/openapi/country-state-city-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: countrystatecity.in
  spf: true
hosts:
- cert_expires: Aug 13 01:14:25 2026 GMT
  host: countrystatecity.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:14:25 2026 GMT
  host: docs.countrystatecity.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:14:25 2026 GMT
  host: api.countrystatecity.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Country State City Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Country State City API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Country State City API
provider_slug: country-state-city-api
slug: country-state-city-api-domain-security
source_filename: country-state-city-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: countrystatecity.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:25 2026 GMT\n  hsts: false\n- host: docs.countrystatecity.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.countrystatecity.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:25 2026 GMT\n  hsts: null\ndomains:\n- domain: countrystatecity.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/security/country-state-city-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Capitals
- Cities
- Countries
- Currencies
- Geography
- Geolocation
- ISO 3166
- JSON
- Phone Codes
- Provinces
- Reference Data
- Regions
- States
- Time Zones
---
