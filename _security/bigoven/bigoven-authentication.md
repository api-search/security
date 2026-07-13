---
api_key_in:
- header
api_specs:
- filename: index
  format: yaml
  label: BigOven Build API
  slug: bigoven-api
  spec_type: OpenAPI
  url: https://api2.bigoven.com/swagger/ui/index
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bigoven Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigOven secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BigOven
provider_slug: bigoven
scheme_count: 2
schemes:
- description: 'Pass your api_key in the header (recommended) or as a URL parameter. For the URL parameter, use api_key. For the header, send it as a header value for: X-BigOven-API-Key'
  in: header
  name: api_key
  parameter: X-BigOven-API-Key
  sources:
  - openapi/bigoven-openapi.yaml
  type: apiKey
- description: Basic HTTP Authentication is used for those endpoint calls where you want to act as a BigOven user -- e.g., to get the list of favorites of a signed-in user, or add items to their grocery list.
  name: basic
  scheme: basic
  sources:
  - openapi/bigoven-openapi.yaml
  type: http
slug: bigoven-authentication
source_filename: bigoven-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigoven-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-BigOven-API-Key\n  description: 'Pass your api_key in the header (recommended) or as a URL parameter. For the\n    URL parameter, use api_key. For the header, send it as a header value for: X-BigOven-API-Key'\n  sources:\n  - openapi/bigoven-openapi.yaml\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic HTTP Authentication is used for those endpoint calls where you want to\n    act as a BigOven user -- e.g., to get the list of favorites of a signed-in user, or add\n    items to their grocery list.\n  sources:\n  - openapi/bigoven-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigoven/refs/heads/main/authentication/bigoven-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Recipes
- Meal Planning
- Grocery Lists
- Nutrition
- Food
- Cooking
---
