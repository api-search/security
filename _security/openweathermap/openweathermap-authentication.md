---
api_key_in:
- query
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
