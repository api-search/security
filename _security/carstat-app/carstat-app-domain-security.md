---
api_specs:
- filename: carstat-app-recalls-api-openapi.yml
  format: yaml
  label: carstat-app Recalls API
  slug: carstat-app-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-recalls-api-openapi.yml
- filename: carstat-app-safety-ratings-api-openapi.yml
  format: yaml
  label: carstat-app Safety Ratings API
  slug: carstat-app-safety-ratings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-safety-ratings-api-openapi.yml
- filename: carstat-app-vehicle-specifications-api-openapi.yml
  format: yaml
  label: carstat-app Vehicle Specifications API
  slug: carstat-app-vehicle-specifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vehicle-specifications-api-openapi.yml
- filename: carstat-app-vin-decoding-api-openapi.yml
  format: yaml
  label: carstat-app VIN Decoding API
  slug: carstat-app-vin-decoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vin-decoding-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carstat.app
  spf: true
hosts:
- cert_expires: Dec  1 07:15:49 2026 GMT
  host: carstat.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carstat App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for carstat-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: carstat-app
provider_slug: carstat-app
slug: carstat-app-domain-security
source_filename: carstat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carstat.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 07:15:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carstat.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/carstat-app/security/carstat-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Data
- API
- Vehicle
---
