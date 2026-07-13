---
api_key_in:
- header
api_specs:
- filename: finout-api-openapi.yml
  format: yaml
  label: Finout
  slug: finout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/openapi/finout-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Finout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finout secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finout
provider_slug: finout
scheme_count: 2
schemes:
- description: The Client ID generated from the Finout Admin Portal under API Tokens.
  in: header
  name: clientId
  parameter: x-finout-client-id
  sources:
  - openapi/finout-api-openapi.yml
  type: apiKey
- description: The Secret Key generated from the Finout Admin Portal under API Tokens. This value is only shown once at generation time.
  in: header
  name: secretKey
  parameter: x-finout-secret-key
  sources:
  - openapi/finout-api-openapi.yml
  type: apiKey
slug: finout-authentication
source_filename: finout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finout-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: x-finout-client-id\n  description: The Client ID generated from the Finout Admin Portal under API Tokens.\n  sources:\n  - openapi/finout-api-openapi.yml\n- name: secretKey\n  type: apiKey\n  in: header\n  parameter: x-finout-secret-key\n  description: The Secret Key generated from the Finout Admin Portal under API Tokens. This\n    value is only shown once at generation time.\n  sources:\n  - openapi/finout-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/authentication/finout-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Budgets
- Costs
- FinOps
---
