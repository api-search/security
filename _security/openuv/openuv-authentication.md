---
api_key_in:
- header
api_specs:
- filename: openuv-account-api-openapi.yml
  format: yaml
  label: OpenUV Account API
  slug: openuv-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/openapi/openuv-account-api-openapi.yml
- filename: openuv-protection-api-openapi.yml
  format: yaml
  label: OpenUV Protection API
  slug: openuv-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/openapi/openuv-protection-api-openapi.yml
- filename: openuv-uv-index-api-openapi.yml
  format: yaml
  label: OpenUV UV Index API
  slug: openuv-uv-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/openapi/openuv-uv-index-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openuv Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenUV secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenUV
provider_slug: openuv
scheme_count: 1
schemes:
- description: OpenUV API key issued from https://www.openuv.io/console
  in: header
  name: ApiKeyAuth
  parameter: x-access-token
  sources:
  - openapi/openuv-openapi.yml
  type: apiKey
slug: openuv-authentication
source_filename: openuv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openuv-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-access-token\n  description: OpenUV API key issued from https://www.openuv.io/console\n  sources:\n  - openapi/openuv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/authentication/openuv-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- UV Index
- Sun
- Solar
- Geolocation
- Forecast
- Public APIs
---
