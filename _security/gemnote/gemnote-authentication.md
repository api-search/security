---
api_key_in:
- header
api_specs:
- filename: gemnote-openapi.yml
  format: yaml
  label: Gemnote API
  slug: gemnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemnote/refs/heads/main/openapi/gemnote-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gemnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemnote secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gemnote
provider_slug: gemnote
scheme_count: 1
schemes:
- description: A token issued by your Gemnote account manager. Sandbox tokens begin with `t_` and production tokens begin with `p_`.
  in: header
  name: AuthorizationToken
  parameter: AUTHORIZATION
  sources:
  - openapi/gemnote-openapi.yml
  type: apiKey
slug: gemnote-authentication
source_filename: gemnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gemnote-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthorizationToken\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  description: A token issued by your Gemnote account manager. Sandbox tokens begin with `t_`\n    and production tokens begin with `p_`.\n  sources:\n  - openapi/gemnote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemnote/refs/heads/main/authentication/gemnote-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Corporate Gifting
- Swag Management
- Branded Merchandise
- Fulfillment
- E-commerce
- Shipping
- Y Combinator
---
