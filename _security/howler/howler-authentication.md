---
api_key_in:
- header
- query
api_specs:
- filename: howler-consumer-portal-openapi.yml
  format: yaml
  label: Howler API v3 (Consumer Portal)
  slug: howler-api-v3-consumer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-consumer-portal-openapi.yml
- filename: howler-webhooks-openapi.yml
  format: yaml
  label: Howler Webhooks v1
  slug: howler-webhooks-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-webhooks-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Howler Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Howler secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Howler
provider_slug: howler
scheme_count: 5
schemes:
- description: OAuth2 authentication for third-party applications
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: /oauth/token
  name: oauth2
  sources:
  - openapi/howler-consumer-portal-openapi.yml
  type: oauth2
- bearerFormat: oauth2
  name: bearer_header
  scheme: bearer
  sources:
  - openapi/howler-consumer-portal-openapi.yml
  type: http
- in: query
  name: bearer_param
  parameter: bearer_token
  sources:
  - openapi/howler-consumer-portal-openapi.yml
  type: apiKey
- description: Basic authentication with email and password
  name: basic_auth
  scheme: basic
  sources:
  - openapi/howler-consumer-portal-openapi.yml
  type: http
- description: API key authentication
  in: header
  name: api_key
  parameter: x-auth-token
  sources:
  - openapi/howler-consumer-portal-openapi.yml
  type: apiKey
slug: howler-authentication
source_filename: howler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/howler-consumer-portal-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 3\n  description: OAuth2 authentication for third-party applications\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- name: bearer_header\n  type: http\n  scheme: bearer\n  bearerFormat: oauth2\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- name: bearer_param\n  type: apiKey\n  in: query\n  parameter: bearer_token\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Basic authentication with email and password\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- name: api_key\n  type:\
  \ apiKey\n  in: header\n  parameter: x-auth-token\n  description: API key authentication\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/authentication/howler-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Events
- Ticketing
- Payments
- Cashless
- RFID
- Event Management
- Fintech
- South Africa
---
