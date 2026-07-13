---
api_key_in: []
api_specs:
- filename: synctera-openapi.json
  format: json
  label: Synctera Platform API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synctera/refs/heads/main/openapi/synctera-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synctera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synctera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synctera
provider_slug: synctera
scheme_count: 1
schemes:
- bearerFormat: api_key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synctera-openapi.json
  type: http
slug: synctera-authentication
source_filename: synctera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synctera-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: api_key\n  sources:\n  - openapi/synctera-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synctera/refs/heads/main/authentication/synctera-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- KYC
---
