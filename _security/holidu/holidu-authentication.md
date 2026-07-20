---
api_key_in:
- header
api_specs:
- filename: holidu-affiliate-api.json
  format: json
  label: Holidu Affiliate API
  slug: holidu-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/openapi/holidu-affiliate-api.json
- filename: holidu-connectivity-api.json
  format: json
  label: Holidu Connectivity API
  slug: holidu-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/openapi/holidu-connectivity-api.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Holidu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holidu secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Holidu
provider_slug: holidu
scheme_count: 5
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/holidu-affiliate-api.json
  type: apiKey
- bearerFormat: JWT
  description: Holidu authenticates to the affiliate using an OAuth 2.0 Bearer Token ([RFC 6750](https://www.rfc-editor.org/rfc/rfc6750)). Token exchange details are agreed upon during onboarding.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/holidu-affiliate-api.json
  type: http
- in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/holidu-connectivity-api.json
  type: apiKey
- flows: []
  name: sec0
  sources:
  - openapi/holidu-hapi-with-oauth20.json
  - openapi/holidu-security-service-with-tokens.json
  type: oauth2
- name: sec0
  scheme: basic
  sources:
  - openapi/holidu-security-service-with-client-credentials.json
  type: http
slug: holidu-authentication
source_filename: holidu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/holidu-affiliate-api.json, openapi/holidu-connectivity-api.json, openapi/holidu-hapi-with-oauth20.json,\n  openapi/holidu-security-service-with-client-credentials.json, openapi/holidu-security-service-with-tokens.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/holidu-affiliate-api.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Holidu authenticates to the affiliate using an OAuth 2.0 Bearer Token ([RFC 6750](https://www.rfc-editor.org/rfc/rfc6750)).\n    Token exchange details are agreed upon during onboarding.\n  sources:\n  - openapi/holidu-affiliate-api.json\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/holidu-connectivity-api.json\n- name: sec0\n  type: oauth2\n  flows: []\n \
  \ sources:\n  - openapi/holidu-hapi-with-oauth20.json\n  - openapi/holidu-security-service-with-tokens.json\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/holidu-security-service-with-client-credentials.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/authentication/holidu-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Travel And Leisure
- Vacation Rentals
- Short-Term Rentals
- Hospitality
- Property Management
- Booking
- Channel Manager
- Connectivity
- Affiliate
---
