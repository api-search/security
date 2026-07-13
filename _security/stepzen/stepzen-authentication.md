---
api_key_in:
- header
api_specs:
- filename: stepzen-admin-openapi.yml
  format: yaml
  label: StepZen Admin API
  slug: stepzen-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stepzen/refs/heads/main/openapi/stepzen-admin-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stepzen Authentication
name_suffix: Authentication
oauth_flows: []
overview: StepZen secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StepZen
provider_slug: stepzen
scheme_count: 1
schemes:
- description: StepZen API key as Bearer token
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/stepzen-admin-openapi.yml
  type: apiKey
slug: stepzen-authentication
source_filename: stepzen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stepzen-admin-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: StepZen API key as Bearer token\n  sources:\n  - openapi/stepzen-admin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepzen/refs/heads/main/authentication/stepzen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backend Integration
- GraphQL
- API Gateway
- REST to GraphQL
- IBM
- Data Federation
---
