---
api_key_in:
- header
api_specs:
- filename: uspto-trademark-search-api-openapi.yml
  format: yaml
  label: USPTO Trademark Search API Endpoints
  slug: uspto-trademark-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-trademark-search-api/refs/heads/main/openapi/uspto-trademark-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uspto Trademark Search Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: USPTO Trademark Search API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: USPTO Trademark Search API
provider_slug: uspto-trademark-search-api
scheme_count: 1
schemes:
- description: RapidAPI subscription key
  in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/uspto-trademark-search-api-openapi.yml
  type: apiKey
slug: uspto-trademark-search-api-authentication
source_filename: uspto-trademark-search-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uspto-trademark-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: RapidAPI subscription key\n  sources:\n  - openapi/uspto-trademark-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto-trademark-search-api/refs/heads/main/authentication/uspto-trademark-search-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Brand
- Brand Protection
- Business
- Data
- Government Data
- Intellectual Property
- Legal
- Search
- Trademark
- USPTO
---
