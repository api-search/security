---
api_specs:
- filename: weatherbit-current-weather-openapi-original.yml
  format: yaml
  label: Weatherbit Current Weather API
  slug: weatherbit-current-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbit/refs/heads/main/openapi/weatherbit-current-weather-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weatherbit.io
  spf: true
hosts:
- cert_expires: Sep 25 23:18:34 2026 GMT
  host: www.weatherbit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:21:33 2026 GMT
  host: api.weatherbit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weatherbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weatherbit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weatherbit
provider_slug: weatherbit
slug: weatherbit-domain-security
source_filename: weatherbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weatherbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:18:34 2026 GMT\n  hsts: false\n- host: api.weatherbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:21:33 2026 GMT\n  hsts: false\ndomains:\n- domain: weatherbit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherbit/refs/heads/main/security/weatherbit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecasting
- Historical Data
- Air Quality
- Alerts
- Agricultural Weather
---
