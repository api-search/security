---
api_key_in:
- header
api_specs:
- filename: lunchbox-core-openapi.yml
  format: yaml
  label: Lunchbox Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-core-openapi.yml
- filename: lunchbox-management-openapi.yml
  format: yaml
  label: Lunchbox Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-management-openapi.yml
- filename: lunchbox-loyalty-openapi.yml
  format: yaml
  label: Lunchbox Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-loyalty-openapi.yml
- filename: lunchbox-pos-openapi.yml
  format: yaml
  label: Lunchbox POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-pos-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lunchbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunchbox secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lunchbox
provider_slug: lunchbox
scheme_count: 2
schemes:
- description: 'Team token passed as: Authorization: Token <team_token>'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/lunchbox-core-openapi.yml
  - openapi/lunchbox-management-openapi.yml
  - openapi/lunchbox-pos-openapi.yml
  type: apiKey
- description: Loyalty engine API key passed in the Api-Key header.
  in: header
  name: apiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/lunchbox-loyalty-openapi.yml
  type: apiKey
slug: lunchbox-authentication
source_filename: lunchbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lunchbox-core-openapi.yml, openapi/lunchbox-loyalty-openapi.yml, openapi/lunchbox-management-openapi.yml,\n  openapi/lunchbox-pos-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Team token passed as: Authorization: Token <team_token>'\n  sources:\n  - openapi/lunchbox-core-openapi.yml\n  - openapi/lunchbox-management-openapi.yml\n  - openapi/lunchbox-pos-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Loyalty engine API key passed in the Api-Key header.\n  sources:\n  - openapi/lunchbox-loyalty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/authentication/lunchbox-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Restaurant
- Online Ordering
- Guest Engagement
- Catering
- Menus
- Orders
- Loyalty
- Enterprise
---
