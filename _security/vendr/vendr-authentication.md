---
api_key_in:
- header
api_specs:
- filename: vendr-openapi.yml
  format: yaml
  label: Vendr OpenPrice API
  slug: vendr-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendr/refs/heads/main/openapi/vendr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vendr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vendr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vendr
provider_slug: vendr
scheme_count: 1
schemes:
- description: API key for authenticating requests. Contact developers@vendr.com to obtain a key.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/vendr-openapi.yml
  type: apiKey
slug: vendr-authentication
source_filename: vendr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vendr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating requests. Contact developers@vendr.com to obtain a\n    key.\n  sources:\n  - openapi/vendr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendr/refs/heads/main/authentication/vendr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pricing
- Procurement
- SaaS
- Software Spend Management
- Negotiation
---
