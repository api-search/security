---
api_specs:
- filename: restcountries-countries-api-openapi.yml
  format: yaml
  label: REST Countries Countries API
  slug: restcountries-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restcountries/refs/heads/main/openapi/restcountries-countries-api-openapi.yml
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
- cert_expires: Sep  2 22:31:48 2026 GMT
  host: api.restcountries.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restcountries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REST Countries, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: REST Countries
provider_slug: restcountries
slug: restcountries-domain-security
source_filename: restcountries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restcountries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:35:35 2026 GMT\n  hsts: false\n- host: api.restcountries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:31:48 2026 GMT\n  hsts: null\ndomains:\n- domain: restcountries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restcountries/refs/heads/main/security/restcountries-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Countries
- Geography
- World Data
- Flags
- Currencies
- Languages
- Population
---
