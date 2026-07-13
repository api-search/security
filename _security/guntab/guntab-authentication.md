---
api_key_in:
- header
api_specs:
- filename: guntab-openapi.yml
  format: yaml
  label: GunTab REST API
  slug: guntab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guntab/refs/heads/main/openapi/guntab-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Guntab Authentication
name_suffix: Authentication
oauth_flows: []
overview: GunTab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GunTab
provider_slug: guntab
scheme_count: 1
schemes:
- description: 'Format: `Token {token_uuid}` issued to verified email users.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/guntab-openapi.yml
  type: apiKey
slug: guntab-authentication
source_filename: guntab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guntab-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format: `Token {token_uuid}` issued to verified email users.'\n  sources:\n  - openapi/guntab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guntab/refs/heads/main/authentication/guntab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Commerce
- Firearms
- Marketplace
- Payments
---
