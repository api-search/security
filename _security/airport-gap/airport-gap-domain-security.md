---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Airport Gap REST API
  slug: airport-gap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airport-gap/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: airportgap.com
  spf: false
hosts:
- cert_expires: Sep 17 14:04:16 2026 GMT
  host: airportgap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airport Gap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airport Gap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Airport Gap
provider_slug: airport-gap
slug: airport-gap-domain-security
source_filename: airport-gap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airportgap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:04:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airportgap.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airport-gap/refs/heads/main/security/airport-gap-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Airports
- Aviation
- Transportation
- IATA
- ICAO
- Distance Calculation
- Geolocation
---
