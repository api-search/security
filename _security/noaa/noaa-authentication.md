---
api_key_in:
- header
api_specs:
- filename: noaa-alerts-api-openapi.yml
  format: yaml
  label: NOAA Alerts API
  slug: noaa-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-alerts-api-openapi.yml
- filename: noaa-aviation-api-openapi.yml
  format: yaml
  label: NOAA Aviation API
  slug: noaa-aviation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-aviation-api-openapi.yml
- filename: noaa-glossary-api-openapi.yml
  format: yaml
  label: NOAA Glossary API
  slug: noaa-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-glossary-api-openapi.yml
- filename: noaa-gridpoints-api-openapi.yml
  format: yaml
  label: NOAA Gridpoints API
  slug: noaa-gridpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-gridpoints-api-openapi.yml
- filename: noaa-icons-api-openapi.yml
  format: yaml
  label: NOAA Icons API
  slug: noaa-icons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-icons-api-openapi.yml
- filename: noaa-navigational-data-api-openapi.yml
  format: yaml
  label: NOAA Navigational Data API
  slug: noaa-navigational-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-navigational-data-api-openapi.yml
- filename: noaa-offices-api-openapi.yml
  format: yaml
  label: NOAA Offices API
  slug: noaa-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-offices-api-openapi.yml
- filename: noaa-points-api-openapi.yml
  format: yaml
  label: NOAA Points API
  slug: noaa-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-points-api-openapi.yml
- filename: noaa-products-api-openapi.yml
  format: yaml
  label: NOAA Products API
  slug: noaa-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-products-api-openapi.yml
- filename: noaa-radar-api-openapi.yml
  format: yaml
  label: NOAA Radar API
  slug: noaa-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-radar-api-openapi.yml
- filename: noaa-radio-api-openapi.yml
  format: yaml
  label: NOAA Radio API
  slug: noaa-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-radio-api-openapi.yml
- filename: noaa-stations-api-openapi.yml
  format: yaml
  label: NOAA Stations API
  slug: noaa-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-stations-api-openapi.yml
- filename: noaa-thumbnails-api-openapi.yml
  format: yaml
  label: NOAA Thumbnails API
  slug: noaa-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-thumbnails-api-openapi.yml
- filename: noaa-weather-data-api-openapi.yml
  format: yaml
  label: NOAA Weather Data API
  slug: noaa-weather-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-weather-data-api-openapi.yml
- filename: noaa-zones-api-openapi.yml
  format: yaml
  label: NOAA Zones API
  slug: noaa-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-zones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Noaa Authentication
name_suffix: Authentication
oauth_flows: []
overview: NOAA secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NOAA
provider_slug: noaa
scheme_count: 2
schemes:
- description: 'We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.

    The API rem'
  in: header
  name: userAgent
  parameter: User-Agent
  sources:
  - openapi/noaa-nws-openapi.yml
  type: apiKey
- description: 'We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.

    The API remains open and free to use and there are no limits imposed based on the X-Api-Key string.'
  in: header
  name: apiKeyAuth
  parameter: API-Key
  sources:
  - openapi/noaa-nws-openapi.yml
  type: apiKey
slug: noaa-authentication
source_filename: noaa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/noaa-nws-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userAgent\n  type: apiKey\n  in: header\n  parameter: User-Agent\n  description: |-\n    We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.\n    The API rem\n  sources:\n  - openapi/noaa-nws-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: |-\n    We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.\n    The API remains open and free to use and there are no\
  \ limits imposed based on the X-Api-Key string.\n  sources:\n  - openapi/noaa-nws-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/authentication/noaa-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Weather
- Climate
- Forecast
- Alerts
- Ocean
- Tides
- Aviation Weather
- Government
- Open Data
- Environmental
---
