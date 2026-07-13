---
api_key_in: []
api_specs:
- filename: thunes-openapi.yml
  format: yaml
  label: Thunes Money Transfer API
  slug: thunes-money-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thunes/refs/heads/main/openapi/thunes-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thunes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thunes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thunes
provider_slug: thunes
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using API key as user-ID and API secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/thunes-openapi.yml
  type: http
slug: thunes-authentication
source_filename: thunes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thunes-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using API key as user-ID and API secret as password.\n  sources:\n  - openapi/thunes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thunes/refs/heads/main/authentication/thunes-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Cross-Border
- Payments
- FX
- Mobile Money
---
