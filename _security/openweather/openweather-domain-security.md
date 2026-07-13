---
api_specs:
- filename: openweather-openapi.yml
  format: yaml
  label: OpenWeather One Call API
  slug: openweather-one-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/openapi/openweather-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openweathermap.org
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: openweathermap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.openweathermap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenWeather, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenWeather
provider_slug: openweather
slug: openweather-domain-security
source_filename: openweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openweathermap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.openweathermap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: openweathermap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/security/openweather-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Air Pollution
- Air Quality
- Climate
- Forecasting
- Weather
---
