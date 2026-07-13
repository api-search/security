---
api_key_in: []
api_specs:
- filename: tibber-graphql-api-openapi.yml
  format: yaml
  label: Tibber GraphQL API
  slug: tibber-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-graphql-api-openapi.yml
- filename: tibber-data-api-openapi.yml
  format: yaml
  label: Tibber Data API
  slug: tibber-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-data-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tibber Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tibber secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tibber
provider_slug: tibber
scheme_count: 2
schemes:
- description: OAuth 2.0 Authorization Code Flow with optional PKCE.
  flows:
  - authorizationUrl: https://thewall.tibber.com/connect/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://thewall.tibber.com/connect/token
  name: oauth2
  sources:
  - openapi/tibber-data-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: Personal access token issued at https://developer.tibber.com/settings/access-token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tibber-graphql-api-openapi.yml
  type: http
slug: tibber-authentication
source_filename: tibber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tibber-data-api-openapi.yml, openapi/tibber-graphql-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thewall.tibber.com/connect/authorize\n    tokenUrl: https://thewall.tibber.com/connect/token\n    scopes: 11\n  description: OAuth 2.0 Authorization Code Flow with optional PKCE.\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Personal access token issued at https://developer.tibber.com/settings/access-token.\n  sources:\n  - openapi/tibber-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/authentication/tibber-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Energy
- SmartHome
- SmartMeter
- ElectricityPricing
- ElectricVehicleCharging
- HeatPump
- SolarInverter
- HomeBattery
- GraphQL
- OAuth2
- Nordic
---
