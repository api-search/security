---
api_key_in:
- header
api_specs:
- filename: einride-auth-openapi-original.yml
  format: yaml
  label: 'Einride Extend: Authentication API'
  slug: einride-extend-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-auth-openapi-original.yml
- filename: einride-book-openapi-original.yml
  format: yaml
  label: 'Einride Extend: Shipment & Booking API'
  slug: einride-extend-shipment-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-book-openapi-original.yml
auth_types:
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Einride Authentication
name_suffix: Authentication
oauth_flows: []
overview: Einride secures its APIs with bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Einride
provider_slug: einride
scheme_count: 1
schemes:
- in: header
  name: Authorization
  parameter: authorization
  scheme: bearer
  sources:
  - openapi/einride-book-openapi-original.yml
  - openapi/einride-auth-openapi-original.yml
  type: http
slug: einride-authentication
source_filename: einride-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  openapi/einride-book-openapi-original.yml, openapi/einride-auth-openapi-original.yml,\n  https://extend.saga.einride.tech\ndocs: https://github.com/einride/extend/blob/master/docs/apis.md\nsummary:\n  types:\n  - bearer\n  api_key_in:\n  - header\n  flow: client-credentials (secret exchange for short-lived bearer token)\nmodel:\n  description: >-\n    Einride Extend uses standard Bearer token authentication. An integration is issued a\n    client ID and client secret by an Einride representative, then exchanges them for a\n    short-lived access token via AuthenticationService_ExchangeSecret. The returned\n    accessToken is sent as `Authorization: Bearer <token>` on all subsequent HTTP (or gRPC)\n    calls and refreshed before its expireTime.\n  token_endpoint_operation: AuthenticationService_ExchangeSecret\n  credential_source: Contact your Einride representative to obtain a client ID and client secret.\nschemes:\n\
  - name: Authorization\n  type: http\n  scheme: bearer\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/einride-book-openapi-original.yml\n  - openapi/einride-auth-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/authentication/einride-authentication.yml
summary_line: bearer · 1 scheme
tags:
- Company
- Sustainable Transport
- Freight
- Logistics
- Autonomous Vehicles
- Electric Vehicles
- Shipping
- gRPC
---
