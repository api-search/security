---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: National Weather Service API
  slug: national-weather-service-api
  spec_type: OpenAPI
  url: https://api.weather.gov/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Weather Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Weather Service secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Weather Service
provider_slug: national-weather-service
scheme_count: 2
schemes:
- description: 'We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.

    The API rem'
  in: header
  name: userAgent
  parameter: User-Agent
  sources:
  - openapi/national-weather-service-openapi.json
  type: apiKey
- description: 'We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.

    The API remains open and free to use and there are no limits imposed based on the X-Api-Key string.'
  in: header
  name: apiKeyAuth
  parameter: API-Key
  sources:
  - openapi/national-weather-service-openapi.json
  type: apiKey
slug: national-weather-service-authentication
source_filename: national-weather-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-weather-service-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userAgent\n  type: apiKey\n  in: header\n  parameter: User-Agent\n  description: |-\n    We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.\n    The API rem\n  sources:\n  - openapi/national-weather-service-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: |-\n    We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.\n    The API remains open\
  \ and free to use and there are no limits imposed based on the X-Api-Key string.\n  sources:\n  - openapi/national-weather-service-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/authentication/national-weather-service-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Forecasting
- Weather
---
