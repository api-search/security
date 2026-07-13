---
api_key_in:
- header
api_specs:
- filename: ravelin-merchant-api-openapi.yml
  format: yaml
  label: Ravelin Merchant API
  slug: ravelin-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-merchant-api-openapi.yml
- filename: ravelin-3ds-server-api-openapi.yml
  format: yaml
  label: Ravelin 3D Secure Server API
  slug: ravelin-3ds-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-3ds-server-api-openapi.yml
- filename: ravelin-callbacks-api-openapi.yml
  format: yaml
  label: Ravelin Callbacks API
  slug: ravelin-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-callbacks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ravelin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ravelin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ravelin
provider_slug: ravelin
scheme_count: 1
schemes:
- description: Secret API key prefixed with `token`.
  in: header
  name: secretApiKey
  parameter: Authorization
  sources:
  - openapi/ravelin-3ds-server-api-openapi.yml
  - openapi/ravelin-merchant-api-openapi.yml
  type: apiKey
slug: ravelin-authentication
source_filename: ravelin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ravelin-3ds-server-api-openapi.yml, openapi/ravelin-merchant-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: secretApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Secret API key prefixed with `token`.\n  sources:\n  - openapi/ravelin-3ds-server-api-openapi.yml\n  - openapi/ravelin-merchant-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/authentication/ravelin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- Fraud Detection
- Chargeback Prevention
- Account Takeover
- 3D Secure
- Risk Scoring
- Payments
- Machine Learning
---
