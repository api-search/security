---
api_key_in:
- header
api_specs:
- filename: togai-openapi.yml
  format: yaml
  label: Togai API
  slug: togai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/togai/refs/heads/main/openapi/togai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Togai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Togai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Togai
provider_slug: togai
scheme_count: 2
schemes:
- bearerFormat: Bearer <credential>
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/togai-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/togai-openapi.yml
  type: apiKey
slug: togai-authentication
source_filename: togai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/togai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer <credential>\n  sources:\n  - openapi/togai-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/togai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/togai/refs/heads/main/authentication/togai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Billing
- Metering
- Usage-Based Pricing
- Revenue Management
- SaaS
- Fintech
---
