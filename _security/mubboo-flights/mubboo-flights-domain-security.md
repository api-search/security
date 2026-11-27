---
api_specs:
- filename: mubboo-flights-context-api-openapi.yml
  format: yaml
  label: Mubboo Flights Context API
  slug: mubboo-flights-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mubboo-flights/openapi/mubboo-flights-context-api-openapi.yml
- filename: mubboo-flights-markdown-api-openapi.yml
  format: yaml
  label: Mubboo Flights Markdown API
  slug: mubboo-flights-markdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mubboo-flights/openapi/mubboo-flights-markdown-api-openapi.yml
- filename: mubboo-flights-routes-api-openapi.yml
  format: yaml
  label: Mubboo Flights Routes API
  slug: mubboo-flights-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mubboo-flights/openapi/mubboo-flights-routes-api-openapi.yml
- filename: mubboo-flights-travel-api-openapi.yml
  format: yaml
  label: Mubboo Flights Travel API
  slug: mubboo-flights-travel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mubboo-flights/openapi/mubboo-flights-travel-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mubboo.flights
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: mubboo.flights
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mubboo Flights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mubboo Flights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mubboo Flights
provider_slug: mubboo-flights
slug: mubboo-flights-domain-security
source_filename: mubboo-flights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mubboo.flights\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mubboo.flights\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mubboo-flights/security/mubboo-flights-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Flights
- Travel
- Search
- Comparison
---
