---
api_key_in:
- header
api_specs:
- filename: zestful-openapi.yml
  format: yaml
  label: Zestful Ingredient Parser API
  slug: zestful
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zestful/refs/heads/main/openapi/zestful-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zestful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zestful secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zestful
provider_slug: zestful
scheme_count: 1
schemes:
- description: API key for authentication. Required for professional and enterprise plans. Sandbox tier uses no authentication.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/zestful-openapi.yml
  type: apiKey
slug: zestful-authentication
source_filename: zestful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zestful-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key for authentication. Required for professional and enterprise plans. Sandbox\n    tier uses no authentication.\n  sources:\n  - openapi/zestful-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zestful/refs/heads/main/authentication/zestful-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food
- Ingredients
- Parsers
- Recipes
- USDA
---
