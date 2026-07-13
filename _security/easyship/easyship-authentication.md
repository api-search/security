---
api_key_in: []
api_specs:
- filename: easyship-openapi.yml
  format: yaml
  label: Easyship API
  slug: easyship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Easyship Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easyship secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Easyship
provider_slug: easyship
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/easyship-openapi.yml
  type: http
slug: easyship-authentication
source_filename: easyship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/easyship-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/easyship-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/authentication/easyship-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Logistics
- Ecommerce
- Fulfillment
- CrossBorder
---
