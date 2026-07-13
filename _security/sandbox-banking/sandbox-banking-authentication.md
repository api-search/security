---
api_key_in:
- header
api_specs:
- filename: sandbox-banking-glyue-openapi.yml
  format: yaml
  label: Glyue Integration Gateway API
  slug: glyue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandbox-banking/refs/heads/main/openapi/sandbox-banking-glyue-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sandbox Banking Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sandbox Banking secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sandbox Banking
provider_slug: sandbox-banking
scheme_count: 1
schemes:
- description: 'Token-based authentication. Include your API token as: Authorization: Token <your-token>'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/sandbox-banking-glyue-openapi.yml
  type: apiKey
slug: sandbox-banking-authentication
source_filename: sandbox-banking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sandbox-banking-glyue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Include your API token as: Authorization: Token\n    <your-token>'\n  sources:\n  - openapi/sandbox-banking-glyue-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandbox-banking/refs/heads/main/authentication/sandbox-banking-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Integration
- Banking
- Core Banking
- Credit Unions
- Financial Services
- Fintech
- Integration Platform
- iPaaS
- Open Banking
---
