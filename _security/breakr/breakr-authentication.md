---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Breakr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breakr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Breakr
provider_slug: breakr
scheme_count: 1
schemes:
- description: 'JWT Bearer token. Enter: **Bearer <your_token>**'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/breakr-openapi.json
  type: apiKey
slug: breakr-authentication
source_filename: breakr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: derived\nsource: openapi/breakr-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Bearer token. Enter: **Bearer <your_token>**'\n  sources:\n  - openapi/breakr-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breakr/refs/heads/main/authentication/breakr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- CreatorEconomy
- Fintech
- Software-as-a-Service
- Payments
---
