---
api_key_in:
- query
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
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openweathermap Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenWeatherMap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenWeatherMap
provider_slug: openweathermap
scheme_count: 1
schemes:
- in: query
  name: appid
  parameter: appid
  sources:
  - openapi/openweathermap-accumulated-parameters-openapi.yml
  - openapi/openweathermap-air-pollution-openapi.yml
  - openapi/openweathermap-current-weather-openapi.yml
  - openapi/openweathermap-forecast-openapi.yml
  - openapi/openweathermap-geocoding-openapi.yml
  - openapi/openweathermap-history-openapi.yml
  - openapi/openweathermap-one-call-openapi.yml
  - openapi/openweathermap-road-risk-openapi.yml
  - openapi/openweathermap-solar-openapi.yml
  - openapi/openweathermap-statistical-weather-openapi.yml
  - openapi/openweathermap-weather-maps-openapi.yml
  - openapi/openweathermap-weather-stations-openapi.yml
  type: apiKey
slug: openweathermap-authentication
source_filename: openweathermap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openweathermap-accumulated-parameters-openapi.yml, openapi/openweathermap-air-pollution-openapi.yml,\n  openapi/openweathermap-current-weather-openapi.yml, openapi/openweathermap-forecast-openapi.yml,\n  openapi/openweathermap-geocoding-openapi.yml, openapi/openweathermap-history-openapi.yml,\n  openapi/openweathermap-one-call-openapi.yml, openapi/openweathermap-road-risk-openapi.yml,\n  openapi/openweathermap-solar-openapi.yml, openapi/openweathermap-statistical-weather-openapi.yml,\n  openapi/openweathermap-weather-maps-openapi.yml, openapi/openweathermap-weather-stations-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: appid\n  type: apiKey\n  in: query\n  parameter: appid\n  sources:\n  - openapi/openweathermap-accumulated-parameters-openapi.yml\n  - openapi/openweathermap-air-pollution-openapi.yml\n  - openapi/openweathermap-current-weather-openapi.yml\n  - openapi/openweathermap-forecast-openapi.yml\n\
  \  - openapi/openweathermap-geocoding-openapi.yml\n  - openapi/openweathermap-history-openapi.yml\n  - openapi/openweathermap-one-call-openapi.yml\n  - openapi/openweathermap-road-risk-openapi.yml\n  - openapi/openweathermap-solar-openapi.yml\n  - openapi/openweathermap-statistical-weather-openapi.yml\n  - openapi/openweathermap-weather-maps-openapi.yml\n  - openapi/openweathermap-weather-stations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/authentication/openweathermap-authentication.yml
summary_line: apiKey · 1 scheme
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
