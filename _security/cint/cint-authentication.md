---
api_key_in:
- header
api_specs:
- filename: cint-demand-openapi.yml
  format: yaml
  label: Cint Exchange Demand API
  slug: cint-exchange-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cint/refs/heads/main/openapi/cint-demand-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cint secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cint
provider_slug: cint
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token used for authentication and authorization. See [Authentication Process](https://developer.cint.com/en/guides#authentication-process) documentation for more information.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cint-demand-openapi.yml
  type: http
- description: API Key Authentication
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/cint-demand-openapi.yml
  type: apiKey
slug: cint-authentication
source_filename: cint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cint-demand-openapi.yml\ndocs: https://developer.cint.com/en/guides#authentication-process\nnote: >-\n  Bearer JWT is the primary scheme; tokens (client credentials) are issued via the\n  onboarding Starter Kit. API Key auth (Authorization header) is also supported.\n  Every request must also send the Cint-API-Version date header.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token used for authentication and authorization. See [Authentication Process](https://developer.cint.com/en/guides#authentication-process)\n    documentation for more information.\n  sources:\n  - openapi/cint-demand-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key Authentication\n  sources:\n  - openapi/cint-demand-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cint/refs/heads/main/authentication/cint-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Market Research
- Survey Sample
- Consumer Insights
- Data Collection
- Ad Measurement
- Marketplace
- Panel
---
