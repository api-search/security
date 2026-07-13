---
api_key_in:
- header
api_specs:
- filename: primer-payments-openapi.yml
  format: yaml
  label: Primer Payments API
  slug: primer-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primer/refs/heads/main/openapi/primer-payments-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Primer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Primer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Primer
provider_slug: primer
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/primer-payments-openapi.yml
  type: apiKey
slug: primer-authentication
source_filename: primer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/primer-payments-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/primer-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primer/refs/heads/main/authentication/primer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- payments
- payment orchestration
- payment processing
- fintech
- fraud detection
- smart routing
- checkout
- payment methods
- reconciliation
- webhooks
---
