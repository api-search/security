---
api_key_in:
- header
api_specs:
- filename: api-overview
  format: yaml
  label: Pinwheel API
  slug: pinwheel-api
  spec_type: OpenAPI
  url: https://docs.pinwheelapi.com/public/reference/api-overview
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinwheel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinwheel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pinwheel
provider_slug: pinwheel
scheme_count: 2
schemes:
- description: API Secret
  in: header
  name: apiSecret
  parameter: X-API-SECRET
  sources:
  - openapi/pinwheel-pinwheel-api-openapi.yml
  type: apiKey
- description: Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pinwheel-pinwheel-api-openapi.yml
  type: http
slug: pinwheel-authentication
source_filename: pinwheel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinwheel-pinwheel-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: X-API-SECRET\n  description: API Secret\n  sources:\n  - openapi/pinwheel-pinwheel-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token\n  sources:\n  - openapi/pinwheel-pinwheel-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/authentication/pinwheel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payroll
- Direct Deposit
- Income Verification
- Employment
- Tax Forms
- Fintech
- Open Finance
- Bill Switching
- Financial Data
---
