---
api_key_in: []
api_specs:
- filename: api.v2.html
  format: yaml
  label: Whiplash API
  slug: whiplash-api
  spec_type: OpenAPI
  url: https://developers.getwhiplash.com/api.v2.html
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Whiplash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whiplash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whiplash
provider_slug: whiplash
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: OAuth 2.0 Bearer token. Obtain via authorization code or client credentials flow. See https://help.whiplash.com/hc/en-us/articles/360050870691-Authentication-for-the-V2-API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/whiplash-openapi.json
  type: http
slug: whiplash-authentication
source_filename: whiplash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whiplash-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: OAuth 2.0 Bearer token. Obtain via authorization code or client credentials flow.\n    See https://help.whiplash.com/hc/en-us/articles/360050870691-Authentication-for-the-V2-API\n  sources:\n  - openapi/whiplash-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/authentication/whiplash-authentication.yml
summary_line: http · 1 scheme
tags:
- Fulfillment
- 3PL
- Logistics
- Ecommerce
- Orders
- Inventory
- Shipments
- Returns
- Warehousing
---
