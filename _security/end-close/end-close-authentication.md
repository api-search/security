---
api_key_in:
- header
api_specs:
- filename: end-close-openapi-original.json
  format: json
  label: End Close API
  slug: end-close-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: End Close Authentication
name_suffix: Authentication
oauth_flows: []
overview: End Close secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: End Close
provider_slug: end-close
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/end-close-openapi-original.json
  type: apiKey
slug: end-close-authentication
source_filename: end-close-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/end-close-openapi-original.json\ndocs: https://endclose.com/docs/authentication.md\nnotes: >-\n  End Close authenticates every request with an API key sent in the X-API-KEY header.\n  Keys are viewed/managed in the Settings section of the End Close dashboard\n  (https://app.endclose.com). Keys are environment-scoped (test vs live).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/end-close-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/authentication/end-close-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Reconciliation
- Payments
- Financial Operations
- Accounting
- Banking
- Data Integration
- Webhooks
- Fintech
---
