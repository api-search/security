---
api_key_in:
- header
api_specs:
- filename: wefitter-app-api-openapi.yml
  format: yaml
  label: WeFitter app API
  slug: wefitter-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-app-api-openapi.yml
- filename: wefitter-challenge-api-openapi.yml
  format: yaml
  label: WeFitter challenge API
  slug: wefitter-challenge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-challenge-api-openapi.yml
- filename: wefitter-connection-api-openapi.yml
  format: yaml
  label: WeFitter connection API
  slug: wefitter-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-connection-api-openapi.yml
- filename: wefitter-insights-api-openapi.yml
  format: yaml
  label: WeFitter insights API
  slug: wefitter-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-insights-api-openapi.yml
- filename: wefitter-loyalty-api-openapi.yml
  format: yaml
  label: WeFitter loyalty API
  slug: wefitter-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-loyalty-api-openapi.yml
- filename: wefitter-notification-api-openapi.yml
  format: yaml
  label: WeFitter notification API
  slug: wefitter-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-notification-api-openapi.yml
- filename: wefitter-profile-api-openapi.yml
  format: yaml
  label: WeFitter profile API
  slug: wefitter-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-profile-api-openapi.yml
- filename: wefitter-team-api-openapi.yml
  format: yaml
  label: WeFitter team API
  slug: wefitter-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-team-api-openapi.yml
- filename: wefitter-token-api-openapi.yml
  format: yaml
  label: WeFitter token API
  slug: wefitter-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-token-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wefitter Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeFitter secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WeFitter
provider_slug: wefitter
scheme_count: 2
schemes:
- description: 'Basic Authentication is used to create administrator bearer tokens.


    Once a bearer token has been made, remove this auth. (''logout'' in Swagger'')'
  name: Basic
  scheme: basic
  sources:
  - openapi/wefitter-openapi-original.json
  type: http
- description: 'Bearer authentication for logged-in profiles.


    When using the GUI, please don''t forget to prefix your bearer tokens with the text ''bearer'', followed by a space.'
  in: header
  name: BearerProfile
  parameter: Authorization
  sources:
  - openapi/wefitter-openapi-original.json
  type: apiKey
slug: wefitter-authentication
source_filename: wefitter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wefitter-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: |-\n    Basic Authentication is used to create administrator bearer tokens.\n\n    Once a bearer token has been made, remove this auth. ('logout' in Swagger')\n  sources:\n  - openapi/wefitter-openapi-original.json\n- name: BearerProfile\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Bearer authentication for logged-in profiles.\n\n    When using the GUI, please don't forget to prefix your bearer tokens with the text 'bearer', followed by a space.\n  sources:\n  - openapi/wefitter-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/authentication/wefitter-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Health
- Fitness
- Wearables
- Health Data
- Wellbeing
- Gamification
- Digital Health
- Insurance
- Activity Tracking
---
