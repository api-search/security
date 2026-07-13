---
api_specs:
- filename: accuweather-openapi-original.yml
  format: yaml
  label: AccuWeather API
  slug: accuweather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/openapi/accuweather-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accuweather.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: developer.accuweather.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: dataservice.accuweather.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accuweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccuWeather, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AccuWeather
provider_slug: accuweather
slug: accuweather-domain-security
source_filename: accuweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.accuweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\n- host: dataservice.accuweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: accuweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/security/accuweather-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
---
