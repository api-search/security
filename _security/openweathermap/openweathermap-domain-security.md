---
api_specs:
- filename: openweathermap-current-weather-openapi.yml
  format: yaml
  label: Current Weather Data API
  slug: current-weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-current-weather-openapi.yml
- filename: openweathermap-forecast-openapi.yml
  format: yaml
  label: Forecast APIs
  slug: forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-forecast-openapi.yml
- filename: openweathermap-one-call-openapi.yml
  format: yaml
  label: One Call API 4.0
  slug: one-call
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-one-call-openapi.yml
- filename: openweathermap-air-pollution-openapi.yml
  format: yaml
  label: Air Pollution API
  slug: air-pollution
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-air-pollution-openapi.yml
- filename: openweathermap-geocoding-openapi.yml
  format: yaml
  label: Geocoding API
  slug: geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-geocoding-openapi.yml
- filename: openweathermap-history-openapi.yml
  format: yaml
  label: Historical Weather API
  slug: history
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-history-openapi.yml
- filename: openweathermap-statistical-weather-openapi.yml
  format: yaml
  label: Statistical Weather Data API
  slug: statistical
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-statistical-weather-openapi.yml
- filename: openweathermap-accumulated-parameters-openapi.yml
  format: yaml
  label: Accumulated Parameters API
  slug: accumulated-parameters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-accumulated-parameters-openapi.yml
- filename: openweathermap-solar-openapi.yml
  format: yaml
  label: Solar Energy APIs
  slug: solar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-solar-openapi.yml
- filename: openweathermap-road-risk-openapi.yml
  format: yaml
  label: Road Risk API
  slug: road-risk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-road-risk-openapi.yml
- filename: openweathermap-weather-stations-openapi.yml
  format: yaml
  label: Weather Stations API
  slug: weather-stations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-weather-stations-openapi.yml
- filename: openweathermap-weather-maps-openapi.yml
  format: yaml
  label: Weather Maps 1.0
  slug: weather-maps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-weather-maps-openapi.yml
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
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: history.openweathermap.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Openweathermap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenWeatherMap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenWeatherMap
provider_slug: openweathermap
slug: openweathermap-domain-security
source_filename: openweathermap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openweathermap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.openweathermap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: history.openweathermap.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: openweathermap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/security/openweathermap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecast
- Climate
- Air Pollution
- Air Quality
- Solar
- Geocoding
- History
- Maps
- Road Risk
- Public APIs
---
