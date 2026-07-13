---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Weather.gov API Web Service
  slug: weather-gov-api-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weather-gov/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weather Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weather.gov secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Weather.gov
provider_slug: weather-gov
scheme_count: 2
schemes:
- description: 'We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.

    The API rem'
  in: header
  name: userAgent
  parameter: User-Agent
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: 'We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.

    The API remains open and free to use and there are no limits imposed based on the X-Api-Key string.'
  in: header
  name: apiKeyAuth
  parameter: API-Key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: weather-gov-authentication
source_filename: weather-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userAgent\n  type: apiKey\n  in: header\n  parameter: User-Agent\n  description: |-\n    We require that all consumers of the API include a User-Agent header in requests. This is due to a high number of scripts exhibiting abusive behavior (intentional or unintentional). We recommend setting the value to something that identifies your application and includes a contact email. This will help us contact you if we notice unusual behavior and also aid in troubleshooting issues.\n    The API rem\n  sources:\n  - openapi/openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: |-\n    We are testing including a more traditional API Key system on certain endpoints.  This is due to a large change in the weather.gov site.\n    The API remains open and free to use and there are no limits imposed based\
  \ on the X-Api-Key string.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weather-gov/refs/heads/main/authentication/weather-gov-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Weather
- Government
- United States
- Forecasting
- Alerts
- Open Data
---
