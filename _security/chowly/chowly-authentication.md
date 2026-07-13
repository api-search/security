---
api_key_in:
- header
api_specs:
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Menu Sync API
  slug: menu-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chowly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chowly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chowly
provider_slug: chowly
scheme_count: 1
schemes:
- description: Per-location Chowly API key provisioned by Chowly. Sent as an API key / bearer credential. The exact header name and scheme are defined in Chowly's partner documentation.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/chowly-openapi.yml
  type: apiKey
slug: chowly-authentication
source_filename: chowly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chowly-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Per-location Chowly API key provisioned by Chowly. Sent as an API key / bearer\n    credential. The exact header name and scheme are defined in Chowly's partner documentation.\n  sources:\n  - openapi/chowly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/authentication/chowly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurants
- Online Ordering
- Delivery
- POS Integration
- Menu Sync
---
