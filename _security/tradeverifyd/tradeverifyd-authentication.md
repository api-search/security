---
api_key_in:
- header
api_specs:
- filename: tradeverifyd-openapi-original.json
  format: json
  label: Tradeverifyd API
  slug: tradeverifyd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tradeverifyd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tradeverifyd secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tradeverifyd
provider_slug: tradeverifyd
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: ocp-apim-subscription-key
  sources:
  - openapi/tradeverifyd-openapi-original.json
  type: apiKey
slug: tradeverifyd-authentication
source_filename: tradeverifyd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tradeverifyd-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: ocp-apim-subscription-key\n  sources:\n  - openapi/tradeverifyd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/authentication/tradeverifyd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Trade Compliance
- Risk Management
- Verifiable Credentials
- Customs
- Entity Resolution
- Logistics
---
