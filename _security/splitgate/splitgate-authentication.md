---
api_key_in: []
api_specs:
- filename: splitgate-matches-api-openapi.yml
  format: yaml
  label: Splitgate Matches API
  slug: splitgate-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-matches-api-openapi.yml
- filename: splitgate-players-api-openapi.yml
  format: yaml
  label: Splitgate Players API
  slug: splitgate-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-players-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Splitgate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Splitgate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Splitgate
provider_slug: splitgate
scheme_count: 1
schemes:
- bearerFormat: jwt
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/splitgate-third-party-openapi-original.yml
  type: http
slug: splitgate-authentication
source_filename: splitgate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/splitgate-third-party-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  sources:\n  - openapi/splitgate-third-party-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/authentication/splitgate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Gaming
- Video Games
- Esports
- Player Statistics
- Leaderboards
- Match Data
- Entertainment
---
