---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Feathery REST API
  slug: feathery-rest-api
  spec_type: OpenAPI
  url: https://api-docs.feathery.io/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Feathery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feathery secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Feathery
provider_slug: feathery
scheme_count: 1
schemes:
- description: 'Token-based authentication. Format: Token <API KEY>'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/feathery-rest-api-openapi.yml
  type: apiKey
slug: feathery-authentication
source_filename: feathery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/feathery-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Format: Token <API KEY>'\n  sources:\n  - openapi/feathery-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/authentication/feathery-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Forms
- Form Builder
- Multi-Step Forms
- Document Intelligence
- AI
- Financial Services
- Insurance
- Wealth Management
- eSignature
- Workflows
- Data Intake
- Submissions
- Payments
- Authentication
---
