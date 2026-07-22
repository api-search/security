---
api_key_in: []
api_specs:
- filename: slope-v4-openapi.json
  format: json
  label: Slope v4 API
  slug: slope-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-v4-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Slope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slope secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slope
provider_slug: slope
scheme_count: 1
schemes:
- description: Basic HTTP authentication using the base64 hash of `public_key:secret_key`.
  name: apiKey
  scheme: basic
  sources:
  - openapi/slope-v4-openapi.json
  type: http
slug: slope-authentication
source_filename: slope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/slope-v4-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: Basic HTTP authentication using the base64 hash of `public_key:secret_key`.\n  sources:\n  - openapi/slope-v4-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/authentication/slope-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- BNPL
- Lending
- Credit
- B2B
- Checkout
---
