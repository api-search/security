---
api_key_in: []
api_specs:
- filename: deliveroo-order-api-openapi.yml
  format: yaml
  label: Deliveroo Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-order-api-openapi.yml
- filename: deliveroo-menu-api-openapi.yml
  format: yaml
  label: Deliveroo Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-menu-api-openapi.yml
- filename: deliveroo-site-api-openapi.yml
  format: yaml
  label: Deliveroo Site API
  slug: site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-site-api-openapi.yml
- filename: deliveroo-catalogue-api-openapi.yml
  format: yaml
  label: Deliveroo Catalogue API
  slug: catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-catalogue-api-openapi.yml
- filename: deliveroo-picking-api-openapi.yml
  format: yaml
  label: Deliveroo Picking API
  slug: picking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-picking-api-openapi.yml
- filename: deliveroo-signature-api-openapi.yml
  format: yaml
  label: Deliveroo Signature API
  slug: signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-signature-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deliveroo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deliveroo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deliveroo
provider_slug: deliveroo
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 client credentials access token obtained from https://auth.developers.deliveroo.com/oauth2/token. Tokens expire after 5 minutes; no refresh tokens are issued.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deliveroo-catalogue-api-openapi.yml
  - openapi/deliveroo-menu-api-openapi.yml
  - openapi/deliveroo-order-api-openapi.yml
  - openapi/deliveroo-picking-api-openapi.yml
  - openapi/deliveroo-signature-api-openapi.yml
  - openapi/deliveroo-site-api-openapi.yml
  type: http
slug: deliveroo-authentication
source_filename: deliveroo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deliveroo-catalogue-api-openapi.yml, openapi/deliveroo-menu-api-openapi.yml,\n  openapi/deliveroo-order-api-openapi.yml, openapi/deliveroo-picking-api-openapi.yml, openapi/deliveroo-signature-api-openapi.yml,\n  openapi/deliveroo-site-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 client credentials access token obtained from https://auth.developers.deliveroo.com/oauth2/token.\n    Tokens expire after 5 minutes; no refresh tokens are issued.\n  sources:\n  - openapi/deliveroo-catalogue-api-openapi.yml\n  - openapi/deliveroo-menu-api-openapi.yml\n  - openapi/deliveroo-order-api-openapi.yml\n  - openapi/deliveroo-picking-api-openapi.yml\n  - openapi/deliveroo-signature-api-openapi.yml\n  - openapi/deliveroo-site-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/authentication/deliveroo-authentication.yml
summary_line: http · 1 scheme
tags:
- Food Delivery
- Grocery
- Marketplace
- Logistics
- Restaurants
---
