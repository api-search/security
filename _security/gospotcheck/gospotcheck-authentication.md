---
api_key_in: []
api_specs:
- filename: gospotcheck-external-openapi.yml
  format: yaml
  label: GoSpotCheck External API
  slug: gospotcheck-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-external-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gospotcheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoSpotCheck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoSpotCheck
provider_slug: gospotcheck
scheme_count: 1
schemes:
- description: 'OAuth2 access token supplied as `Authorization: Bearer <token>`. Tokens are issued by GoSpotCheck; contact your Customer Success Manager or support@gospotcheck.com to obtain one.'
  name: oauth2Bearer
  scheme: bearer
  sources:
  - openapi/gospotcheck-external-openapi.yml
  type: http
slug: gospotcheck-authentication
source_filename: gospotcheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gospotcheck-external-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth2Bearer\n  type: http\n  scheme: bearer\n  description: 'OAuth2 access token supplied as `Authorization: Bearer <token>`. Tokens are\n    issued by GoSpotCheck; contact your Customer Success Manager or support@gospotcheck.com\n    to obtain one.'\n  sources:\n  - openapi/gospotcheck-external-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/authentication/gospotcheck-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Retail Execution
- Field Service
- Data Collection
- Surveys
- Merchandising
- CPG
- Mobile
---
