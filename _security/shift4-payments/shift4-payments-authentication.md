---
api_key_in: []
api_specs:
- filename: shift4-api-openapi.yml
  format: yaml
  label: Shift4 Payments API
  slug: shift4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/main/openapi/shift4-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shift4 Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shift4 Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shift4 Payments
provider_slug: shift4-payments
scheme_count: 1
schemes:
- description: Use your secret API key as the username with an empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/shift4-api-openapi.yml
  type: http
slug: shift4-payments-authentication
source_filename: shift4-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shift4-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Use your secret API key as the username with an empty password.\n  sources:\n  - openapi/shift4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/authentication/shift4-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Commerce
- Checkout
---
