---
api_key_in:
- header
api_specs:
- filename: unfi-supplier-openapi.yml
  format: yaml
  label: UNFI Harmony Core API
  slug: unfi-harmony-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-natural-foods/main/openapi/unfi-supplier-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: United Natural Foods Authentication
name_suffix: Authentication
oauth_flows: []
overview: United Natural Foods (UNFI) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United Natural Foods (UNFI)
provider_slug: united-natural-foods
scheme_count: 1
schemes:
- description: UNFI supplier API key
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/unfi-supplier-openapi.yml
  type: apiKey
slug: united-natural-foods-authentication
source_filename: united-natural-foods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unfi-supplier-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: UNFI supplier API key\n  sources:\n  - openapi/unfi-supplier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-natural-foods/refs/heads/main/authentication/united-natural-foods-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food Distribution
- Wholesale
- Natural Foods
- Supply Chain
- Fortune 500
---
