---
api_key_in:
- header
api_specs:
- filename: collectors-psa-openapi-original.json
  format: json
  label: PSA Public API
  slug: psa-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/openapi/collectors-psa-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Collectors Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collectors secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Collectors
provider_slug: collectors
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/collectors-psa-openapi-original.json
  type: apiKey
slug: collectors-authentication
source_filename: collectors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/collectors-psa-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/collectors-psa-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/authentication/collectors-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplace
- Collectibles
- Authentication
- Grading
- Trading Cards
- Verification
---
