---
api_key_in: []
api_specs:
- filename: vistra-incorporations-openapi.yml
  format: yaml
  label: Vistra Incorporations API
  slug: incorporations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vistra/refs/heads/main/openapi/vistra-incorporations-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vistra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vistra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vistra
provider_slug: vistra
scheme_count: 1
schemes:
- description: OAuth2 bearer token obtained from the Vistra Developer Portal. Include in the Authorization header as "Bearer {token}".
  name: OAuth2Bearer
  scheme: bearer
  sources:
  - openapi/vistra-incorporations-openapi.yml
  type: http
slug: vistra-authentication
source_filename: vistra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vistra-incorporations-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth2Bearer\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token obtained from the Vistra Developer Portal. Include in the\n    Authorization header as \"Bearer {token}\".\n  sources:\n  - openapi/vistra-incorporations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vistra/refs/heads/main/authentication/vistra-authentication.yml
summary_line: http · 1 scheme
tags:
- Compliance
- Corporate Services
- Entity Management
- Finance
- Fortune 500
- Legal
---
