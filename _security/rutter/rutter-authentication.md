---
api_key_in: []
api_specs:
- filename: rutter-unified-api-openapi.yml
  format: yaml
  label: Rutter Unified API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter/refs/heads/main/openapi/rutter-unified-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rutter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rutter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rutter
provider_slug: rutter
scheme_count: 1
schemes:
- description: Use client_id as username and client_secret as password. Encode as base64(client_id:client_secret).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/rutter-unified-api-openapi.yml
  type: http
slug: rutter-authentication
source_filename: rutter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rutter-unified-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use client_id as username and client_secret as password. Encode as base64(client_id:client_secret).\n  sources:\n  - openapi/rutter-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rutter/refs/heads/main/authentication/rutter-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- B2B
- Commerce
- Financial Data
- Payments
- Unified API
---
