---
api_key_in: []
api_specs:
- filename: omniful-inc-openapi.yml
  format: yaml
  label: Omniful Integration APIs
  slug: omniful-integration-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omniful-inc/refs/heads/main/openapi/omniful-inc-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Omniful Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omniful, Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Omniful, Inc.
provider_slug: omniful-inc
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/omniful-inc-openapi.yml
  type: http
slug: omniful-inc-authentication
source_filename: omniful-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/omniful-inc-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/omniful-inc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omniful-inc/refs/heads/main/authentication/omniful-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Supply Chain
- Fulfillment
- Order Management
- Warehouse Management
- Transportation Management
- Inventory
- Returns
- E-commerce
- Logistics
---
