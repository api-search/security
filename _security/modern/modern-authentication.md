---
api_key_in: []
api_specs:
- filename: modern-partner-api-openapi.yml
  format: yaml
  label: MODERN Partner API
  slug: modern-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern/refs/heads/main/openapi/modern-partner-api-openapi.yml
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Modern Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modern secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Modern
provider_slug: modern
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/modern-partner-api-openapi.yml
  type: http
  used_by:
  - POST /token
- name: bearerAuth
  scheme: bearer
  scope: single-franchise
  sources:
  - openapi/modern-partner-api-openapi.yml
  token_lifetime_hours: 24
  type: http
  used_by:
  - all /v1/* endpoints
slug: modern-authentication
source_filename: modern-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.modernis.com/ (MODERN Partner API published documentation)\nsummary:\n  types: [http-basic, http-bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Two-step auth. Franchise username/password are exchanged via HTTP Basic auth\n    against POST /token to obtain a bearer access token. All other endpoints require\n    the bearer token. Tokens are valid for 24 hours and scoped to a single franchise;\n    partners receive a separate username/password per franchise they act on behalf of.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    used_by: [POST /token]\n    sources: [openapi/modern-partner-api-openapi.yml]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    token_lifetime_hours: 24\n    scope: single-franchise\n    used_by: [all /v1/* endpoints]\n    sources: [openapi/modern-partner-api-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern/refs/heads/main/authentication/modern-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Heavy Equipment
- Dealership
- Field Service
- Work Orders
- Customer Communications
- Notifications
- Partner API
---
