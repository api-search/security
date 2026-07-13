---
api_specs:
- filename: openapi.json
  format: json
  label: National Weather Service API
  slug: national-weather-service-api
  spec_type: OpenAPI
  url: https://api.weather.gov/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weather.gov
  spf: false
hosts:
- cert_expires: Aug 24 17:22:04 2026 GMT
  host: www.weather.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:22:04 2026 GMT
  host: api.weather.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Weather Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Weather Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: National Weather Service
provider_slug: national-weather-service
slug: national-weather-service-domain-security
source_filename: national-weather-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weather.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/security/national-weather-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Forecasting
- Weather
---
