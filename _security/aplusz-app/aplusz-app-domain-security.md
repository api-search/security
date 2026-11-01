---
api_specs:
- filename: aplusz-app-cities-api-openapi.yml
  format: yaml
  label: aplusz-app Cities API
  slug: aplusz-app-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-cities-api-openapi.yml
- filename: aplusz-app-fare-api-openapi.yml
  format: yaml
  label: aplusz-app Fare API
  slug: aplusz-app-fare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-fare-api-openapi.yml
- filename: aplusz-app-health-api-openapi.yml
  format: yaml
  label: aplusz-app Health API
  slug: aplusz-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-health-api-openapi.yml
- filename: aplusz-app-routes-api-openapi.yml
  format: yaml
  label: aplusz-app Routes API
  slug: aplusz-app-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-routes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aplusz.app
  spf: true
hosts:
- cert_expires: Dec 15 23:46:03 2026 GMT
  host: aplusz.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aplusz App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aplusz-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aplusz-app
provider_slug: aplusz-app
slug: aplusz-app-domain-security
source_filename: aplusz-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aplusz.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aplusz.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aplusz-app/security/aplusz-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Airfare
- Search
- Free
- Booking
---
