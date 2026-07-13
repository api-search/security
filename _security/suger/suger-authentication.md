---
api_key_in:
- header
api_specs:
- filename: suger-openapi.yml
  format: yaml
  label: Suger API
  slug: suger
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Suger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suger secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suger
provider_slug: suger
scheme_count: 1
schemes:
- description: API Key for authorization in format of <Key *****>.
  in: header
  name: APIKeyAuth
  parameter: Authorization
  sources:
  - openapi/suger-openapi.yml
  type: apiKey
slug: suger-authentication
source_filename: suger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suger-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key for authorization in format of <Key *****>.\n  sources:\n  - openapi/suger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/authentication/suger-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Marketplace
- GTM
- SaaS
- Billing
- Entitlement
- Revenue
- Co-Sell
---
