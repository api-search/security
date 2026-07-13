---
api_key_in:
- header
api_specs:
- filename: lithic-openapi.yml
  format: yaml
  label: Lithic REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic/refs/heads/main/openapi/lithic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lithic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lithic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lithic
provider_slug: lithic
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/lithic-openapi.yml
  type: apiKey
slug: lithic-authentication
source_filename: lithic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lithic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/lithic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithic/refs/heads/main/authentication/lithic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance
---
