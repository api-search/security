---
api_key_in:
- header
api_specs:
- filename: noaa-gov-alerts-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Alerts API
  slug: noaa-gov-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-alerts-api-openapi.yml
- filename: noaa-gov-aviation-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Aviation API
  slug: noaa-gov-aviation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-aviation-api-openapi.yml
- filename: noaa-gov-glossary-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Glossary API
  slug: noaa-gov-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-glossary-api-openapi.yml
- filename: noaa-gov-gridpoints-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Gridpoints API
  slug: noaa-gov-gridpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-gridpoints-api-openapi.yml
- filename: noaa-gov-icons-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Icons API
  slug: noaa-gov-icons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-icons-api-openapi.yml
- filename: noaa-gov-offices-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Offices API
  slug: noaa-gov-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-offices-api-openapi.yml
- filename: noaa-gov-points-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Points API
  slug: noaa-gov-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-points-api-openapi.yml
- filename: noaa-gov-products-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Products API
  slug: noaa-gov-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-products-api-openapi.yml
- filename: noaa-gov-radar-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Radar API
  slug: noaa-gov-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-radar-api-openapi.yml
- filename: noaa-gov-radio-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Radio API
  slug: noaa-gov-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-radio-api-openapi.yml
- filename: noaa-gov-stations-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Stations API
  slug: noaa-gov-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-stations-api-openapi.yml
- filename: noaa-gov-thumbnails-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Thumbnails API
  slug: noaa-gov-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-thumbnails-api-openapi.yml
- filename: noaa-gov-zones-api-openapi.yml
  format: yaml
  label: NOAA — National Oceanic and Atmospheric Administration Zones API
  slug: noaa-gov-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/openapi/noaa-gov-zones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Noaa Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: NOAA — National Oceanic and Atmospheric Administration secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NOAA — National Oceanic and Atmospheric Administration
provider_slug: noaa-gov
scheme_count: 2
schemes:
- description: 'We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.

    The API rem'
  in: header
  name: userAgent
  parameter: User-Agent
  sources:
  - openapi/weather-gov-api-openapi.json
  type: apiKey
- description: 'We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.

    The API remains open and free to use and there are no limits imposed based on the X-Api-Key string.'
  in: header
  name: apiKeyAuth
  parameter: API-Key
  sources:
  - openapi/weather-gov-api-openapi.json
  type: apiKey
slug: noaa-gov-authentication
source_filename: noaa-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weather-gov-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userAgent\n  type: apiKey\n  in: header\n  parameter: User-Agent\n  description: |-\n    We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.\n    The API rem\n  sources:\n  - openapi/weather-gov-api-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: |-\n    We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.\n    The API remains open and free to use\
  \ and there are no limits imposed based on the X-Api-Key string.\n  sources:\n  - openapi/weather-gov-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/authentication/noaa-gov-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Weather
- Climate
- Ocean
- Space Weather
- Government
- Open Data
- Forecast
- Marine
- Atmospheric
- Hydrology
- Satellite
- Fisheries
- Aviation
- Emergency Management
---
