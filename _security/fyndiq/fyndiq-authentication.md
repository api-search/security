---
api_key_in: []
api_specs:
- filename: fyndiq-merchant-api-openapi.yml
  format: yaml
  label: Fyndiq Merchant API
  slug: fyndiq-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyndiq/refs/heads/main/openapi/fyndiq-merchant-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fyndiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fyndiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fyndiq
provider_slug: fyndiq
scheme_count: 1
schemes:
- description: Base64-encoded `merchantID:token`.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fyndiq-merchant-api-openapi.yml
  type: http
slug: fyndiq-authentication
source_filename: fyndiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fyndiq-merchant-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded `merchantID:token`.\n  sources:\n  - openapi/fyndiq-merchant-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyndiq/refs/heads/main/authentication/fyndiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Marketplace
- E-Commerce
- Retail
- Products
- Orders
- Sweden
---
