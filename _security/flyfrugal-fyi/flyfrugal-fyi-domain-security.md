---
api_specs:
- filename: flyfrugal-fyi-calendar-api-openapi.yml
  format: yaml
  label: Fly Frugal Calendar API
  slug: flyfrugal-fyi-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-calendar-api-openapi.yml
- filename: flyfrugal-fyi-catalog-api-openapi.yml
  format: yaml
  label: Fly Frugal Catalog API
  slug: flyfrugal-fyi-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-catalog-api-openapi.yml
- filename: flyfrugal-fyi-deals-api-openapi.yml
  format: yaml
  label: Fly Frugal Deals API
  slug: flyfrugal-fyi-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-deals-api-openapi.yml
- filename: flyfrugal-fyi-history-api-openapi.yml
  format: yaml
  label: Fly Frugal History API
  slug: flyfrugal-fyi-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-history-api-openapi.yml
- filename: flyfrugal-fyi-itineraries-api-openapi.yml
  format: yaml
  label: Fly Frugal Itineraries API
  slug: flyfrugal-fyi-itineraries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-itineraries-api-openapi.yml
- filename: flyfrugal-fyi-weather-api-openapi.yml
  format: yaml
  label: Fly Frugal Weather API
  slug: flyfrugal-fyi-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flyfrugal.fyi
  spf: true
hosts:
- cert_expires: Dec 27 23:25:13 2026 GMT
  host: flyfrugal.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fly Frugal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fly Frugal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fly Frugal
provider_slug: flyfrugal-fyi
slug: flyfrugal-fyi-domain-security
source_filename: flyfrugal-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyfrugal.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:25:13 2026 GMT\n  hsts: false\ndomains:\n- domain: flyfrugal.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flyfrugal-fyi/security/flyfrugal-fyi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Data
- MCP
- Flight Deals
- Company
---
