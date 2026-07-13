---
api_key_in:
- header
api_specs:
- filename: v2api.yaml
  format: yaml
  label: Sezzle API v2
  slug: sezzle-api-v2
  spec_type: OpenAPI
  url: https://gateway.sezzle.com/v2api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sezzle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sezzle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sezzle
provider_slug: sezzle
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/sezzle-v2-openapi.yaml
  type: apiKey
slug: sezzle-authentication
source_filename: sezzle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sezzle-v2-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/sezzle-v2-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sezzle/refs/heads/main/authentication/sezzle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Buy Now Pay Later
- BNPL
- Payments
- Installments
- Fintech
- Merchant Integration
- Checkout
---
