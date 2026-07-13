---
api_specs:
- filename: weatherapi-openapi-original.yml
  format: yaml
  label: WeatherAPI
  slug: weatherapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/openapi/weatherapi-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weatherapi.com
  spf: true
hosts:
- cert_expires: Oct  9 03:04:41 2026 GMT
  host: www.weatherapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:03:40 2026 GMT
  host: api.weatherapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weatherapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeatherAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WeatherAPI
provider_slug: weatherapi
slug: weatherapi-domain-security
source_filename: weatherapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weatherapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:04:41 2026 GMT\n  hsts: false\n- host: api.weatherapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:03:40 2026 GMT\n  hsts: false\ndomains:\n- domain: weatherapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/security/weatherapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecast
- History
- Marine
- Astronomy
- Geolocation
- Sports
- Alerts
- Public APIs
---
