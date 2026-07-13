---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: Currents News API
  slug: currents-news-api
  spec_type: OpenAPI
  url: https://currentsapi.services/json/swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Currentsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Currents API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Currents API
provider_slug: currentsapi
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/currentsapi-openapi.json
  type: apiKey
slug: currentsapi-authentication
source_filename: currentsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/currentsapi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/currentsapi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currentsapi/refs/heads/main/authentication/currentsapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media
- Search
- REST
- Real-Time
---
