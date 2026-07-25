---
api_key_in:
- header
api_specs:
- filename: visteon-audio-api-openapi.yml
  format: yaml
  label: Visteon Audio API
  slug: visteon-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-audio-api-openapi.yml
- filename: visteon-media-api-openapi.yml
  format: yaml
  label: Visteon Media API
  slug: visteon-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-media-api-openapi.yml
- filename: visteon-navigation-api-openapi.yml
  format: yaml
  label: Visteon Navigation API
  slug: visteon-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-navigation-api-openapi.yml
- filename: visteon-phone-api-openapi.yml
  format: yaml
  label: Visteon Phone API
  slug: visteon-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-phone-api-openapi.yml
- filename: visteon-screen-management-api-openapi.yml
  format: yaml
  label: Visteon Screen Management API
  slug: visteon-screen-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-screen-management-api-openapi.yml
- filename: visteon-vehicle-api-openapi.yml
  format: yaml
  label: Visteon Vehicle API
  slug: visteon-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-vehicle-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Visteon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Visteon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Visteon
provider_slug: visteon
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Phoenix-API-Key
  sources:
  - openapi/visteon-phoenix-openapi.yml
  type: apiKey
slug: visteon-authentication
source_filename: visteon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/visteon-phoenix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Phoenix-API-Key\n  sources:\n  - openapi/visteon-phoenix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/authentication/visteon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Connected Car
- Infotainment
- IoT
- Fortune 500
---
