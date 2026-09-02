---
api_key_in:
- header
api_specs:
- filename: cuboh-locations-api-openapi.yml
  format: yaml
  label: Cuboh Locations API
  slug: cuboh-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-locations-api-openapi.yml
- filename: cuboh-menu-api-openapi.yml
  format: yaml
  label: Cuboh Menu API
  slug: cuboh-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-menu-api-openapi.yml
- filename: cuboh-orders-api-openapi.yml
  format: yaml
  label: Cuboh Orders API
  slug: cuboh-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-orders-api-openapi.yml
- filename: cuboh-webhooks-api-openapi.yml
  format: yaml
  label: Cuboh Webhooks API
  slug: cuboh-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-webhooks-api-openapi.yml
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
- Point-of-Sale
- Order Aggregation
---
