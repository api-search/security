---
api_key_in:
- header
api_specs:
- filename: adopets-external-openapi.yml
  format: yaml
  label: Adopets External API
  slug: adopets-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/openapi/adopets-external-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adopets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adopets secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adopets
provider_slug: adopets
scheme_count: 2
schemes:
- description: Organization API key issued by Adopets, sent on every request.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/adopets-external-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Per-session token (data.authorization) returned by system-auth/connect.
  name: sessionBearer
  scheme: bearer
  sources:
  - openapi/adopets-external-openapi.yml
  type: http
slug: adopets-authentication
source_filename: adopets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/adopets-external-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Organization API key issued by Adopets, sent on every request.\n  sources:\n  - openapi/adopets-external-openapi.yml\n- name: sessionBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Per-session token (data.authorization) returned by system-auth/connect.\n  sources:\n  - openapi/adopets-external-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/authentication/adopets-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Pet Adoption
- Animal Welfare
- Shelters and Rescues
- Adoption Management
- Payments
- Nonprofit Technology
- SaaS
- Company
---
