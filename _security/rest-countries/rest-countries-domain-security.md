---
api_specs:
- filename: rest-countries-openapi.yml
  format: yaml
  label: REST Countries
  slug: rest-countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: restcountries.com
  spf: true
hosts:
- cert_expires: Sep  8 20:35:35 2026 GMT
  host: restcountries.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rest Countries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REST Countries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: REST Countries
provider_slug: rest-countries
slug: rest-countries-domain-security
source_filename: rest-countries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restcountries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:35:35 2026 GMT\n  hsts: false\ndomains:\n- domain: restcountries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/security/rest-countries-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Countries
- Geocoding
- Geography
- ISO 3166
- Open Source
- Public APIs
- Reference Data
- Currencies
- Languages
- Capitals
- Regions
- Subregions
- Translations
---
