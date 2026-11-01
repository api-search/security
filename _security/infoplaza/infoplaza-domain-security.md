---
api_specs:
- filename: infoplaza-geo-api-openapi.yml
  format: yaml
  label: Infoplaza Geo API
  slug: infoplaza-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-geo-api-openapi.yml
- filename: infoplaza-marine-api-openapi.yml
  format: yaml
  label: Infoplaza Marine API
  slug: infoplaza-marine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-marine-api-openapi.yml
- filename: infoplaza-observations-api-openapi.yml
  format: yaml
  label: Infoplaza Observations API
  slug: infoplaza-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-observations-api-openapi.yml
- filename: infoplaza-port-api-openapi.yml
  format: yaml
  label: Infoplaza Port API
  slug: infoplaza-port-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-port-api-openapi.yml
- filename: infoplaza-storms-api-openapi.yml
  format: yaml
  label: Infoplaza Storms API
  slug: infoplaza-storms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-storms-api-openapi.yml
- filename: infoplaza-traffic-api-openapi.yml
  format: yaml
  label: Infoplaza Traffic API
  slug: infoplaza-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-traffic-api-openapi.yml
- filename: infoplaza-transit-api-openapi.yml
  format: yaml
  label: Infoplaza Transit API
  slug: infoplaza-transit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-transit-api-openapi.yml
- filename: infoplaza-weather-api-openapi.yml
  format: yaml
  label: Infoplaza Weather API
  slug: infoplaza-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infoplaza.com
  spf: true
hosts:
- cert_expires: Jan  9 06:58:24 2027 GMT
  host: infoplaza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Infoplaza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infoplaza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infoplaza
provider_slug: infoplaza
slug: infoplaza-domain-security
source_filename: infoplaza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infoplaza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:58:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infoplaza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/infoplaza/security/infoplaza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Mobility
- Forecasting
- EventPlanning
- DataAnalytics
- Weather Data
- Marine
- Meteorology
- Geospatial
---
