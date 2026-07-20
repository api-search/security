---
api_key_in:
- header
api_specs:
- filename: golden-recursion-openapi-original.json
  format: json
  label: Golden API v2
  slug: golden-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/openapi/golden-recursion-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Golden Recursion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Golden Recursion secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Golden Recursion
provider_slug: golden-recursion
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/golden-recursion-openapi-original.json
  type: apiKey
slug: golden-recursion-authentication
source_filename: golden-recursion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/golden-recursion-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/golden-recursion-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/authentication/golden-recursion-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Knowledge Graph
- Data Enrichment
- Entity Data
- Company Data
- Artificial Intelligence
- Semantic Web
- Data
---
