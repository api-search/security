---
api_key_in:
- cookie
- header
api_specs:
- filename: vendure-shop-api-openapi.yml
  format: yaml
  label: Vendure Shop GraphQL API
  slug: shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-shop-api-openapi.yml
- filename: vendure-admin-api-openapi.yml
  format: yaml
  label: Vendure Admin GraphQL API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-admin-api-openapi.yml
- filename: vendure-asset-server-openapi.yml
  format: yaml
  label: Vendure Asset Server REST API
  slug: asset-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-asset-server-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vendure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vendure secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vendure
provider_slug: vendure
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vendure-admin-api-openapi.yml
  - openapi/vendure-shop-api-openapi.yml
  type: http
- in: cookie
  name: CookieAuth
  parameter: session
  sources:
  - openapi/vendure-admin-api-openapi.yml
  - openapi/vendure-shop-api-openapi.yml
  type: apiKey
- in: header
  name: ChannelToken
  parameter: vendure-token
  sources:
  - openapi/vendure-admin-api-openapi.yml
  - openapi/vendure-shop-api-openapi.yml
  type: apiKey
slug: vendure-authentication
source_filename: vendure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vendure-admin-api-openapi.yml, openapi/vendure-shop-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/vendure-admin-api-openapi.yml\n  - openapi/vendure-shop-api-openapi.yml\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session\n  sources:\n  - openapi/vendure-admin-api-openapi.yml\n  - openapi/vendure-shop-api-openapi.yml\n- name: ChannelToken\n  type: apiKey\n  in: header\n  parameter: vendure-token\n  sources:\n  - openapi/vendure-admin-api-openapi.yml\n  - openapi/vendure-shop-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/authentication/vendure-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Commerce
- Headless Commerce
- eCommerce
- GraphQL
- Open Source
- TypeScript
- NestJS
- B2B
- B2C
- Storefront
- Plugins
---
