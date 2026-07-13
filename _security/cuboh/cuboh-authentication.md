---
api_key_in:
- header
api_specs:
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Menu API
  slug: menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Merchant Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cuboh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuboh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cuboh
provider_slug: cuboh
scheme_count: 1
schemes:
- description: 'Partner integration token supplied by Cuboh, sent as `Authorization: Token <your token>`. Tokens are unique per partner and a single token authenticates all endpoints.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/cuboh-openapi.yml
  type: apiKey
slug: cuboh-authentication
source_filename: cuboh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cuboh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Partner integration token supplied by Cuboh, sent as `Authorization: Token <your\n    token>`. Tokens are unique per partner and a single token authenticates all endpoints.'\n  sources:\n  - openapi/cuboh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/authentication/cuboh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Online Ordering
- Delivery
- POS
- Order Aggregation
---
