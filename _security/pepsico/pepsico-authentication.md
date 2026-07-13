---
api_key_in: []
api_specs:
- filename: pepsico-pepsico-api-openapi.yml
  format: yaml
  label: PepsiCo API
  slug: pepsico-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pepsico/refs/heads/main/openapi/pepsico-pepsico-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pepsico Authentication
name_suffix: Authentication
oauth_flows: []
overview: PepsiCo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PepsiCo
provider_slug: pepsico
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pepsico-pepsico-api-openapi.yml
  type: http
slug: pepsico-authentication
source_filename: pepsico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pepsico-pepsico-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/pepsico-pepsico-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepsico/refs/heads/main/authentication/pepsico-authentication.yml
summary_line: http · 1 scheme
tags:
- Beverages
- Food
- Retail
- Supply Chain
- Fortune 100
---
