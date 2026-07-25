---
api_specs:
- filename: openweathermap-accumulated-parameters-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Accumulated Parameters API
  slug: openweathermap-accumulated-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-accumulated-parameters-api-openapi.yml
- filename: openweathermap-air-pollution-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Air Pollution API
  slug: openweathermap-air-pollution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-air-pollution-api-openapi.yml
- filename: openweathermap-current-weather-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Current Weather API
  slug: openweathermap-current-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-current-weather-api-openapi.yml
- filename: openweathermap-forecast-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Forecast API
  slug: openweathermap-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-forecast-api-openapi.yml
- filename: openweathermap-geocoding-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Geocoding API
  slug: openweathermap-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-geocoding-api-openapi.yml
- filename: openweathermap-history-api-openapi.yml
  format: yaml
  label: OpenWeatherMap History API
  slug: openweathermap-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-history-api-openapi.yml
- filename: openweathermap-measurements-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Measurements API
  slug: openweathermap-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-measurements-api-openapi.yml
- filename: openweathermap-one-call-api-openapi.yml
  format: yaml
  label: OpenWeatherMap One Call API
  slug: openweathermap-one-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-one-call-api-openapi.yml
- filename: openweathermap-road-risk-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Road Risk API
  slug: openweathermap-road-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-road-risk-api-openapi.yml
- filename: openweathermap-solar-irradiance-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Solar Irradiance API
  slug: openweathermap-solar-irradiance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-solar-irradiance-api-openapi.yml
- filename: openweathermap-solar-panels-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Solar Panels API
  slug: openweathermap-solar-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-solar-panels-api-openapi.yml
- filename: openweathermap-stations-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Stations API
  slug: openweathermap-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-stations-api-openapi.yml
- filename: openweathermap-statistical-weather-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Statistical Weather API
  slug: openweathermap-statistical-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-statistical-weather-api-openapi.yml
- filename: openweathermap-weather-maps-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Weather Maps API
  slug: openweathermap-weather-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-weather-maps-api-openapi.yml
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
