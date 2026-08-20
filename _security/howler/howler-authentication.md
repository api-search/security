---
api_key_in:
- header
- query
api_specs:
- filename: howler-artists-api-openapi.yml
  format: yaml
  label: Howler Artists API
  slug: howler-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-artists-api-openapi.yml
- filename: howler-assign-ticket-api-openapi.yml
  format: yaml
  label: Howler Assign Ticket API
  slug: howler-assign-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-assign-ticket-api-openapi.yml
- filename: howler-bank-account-api-openapi.yml
  format: yaml
  label: Howler Bank Account API
  slug: howler-bank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-bank-account-api-openapi.yml
- filename: howler-basic-authentication-api-openapi.yml
  format: yaml
  label: Howler Basic Authentication API
  slug: howler-basic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-basic-authentication-api-openapi.yml
- filename: howler-cashless-tags-api-openapi.yml
  format: yaml
  label: Howler Cashless Tags API
  slug: howler-cashless-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashless-tags-api-openapi.yml
- filename: howler-cashout-api-openapi.yml
  format: yaml
  label: Howler Cashout API
  slug: howler-cashout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashout-api-openapi.yml
- filename: howler-email-otp-api-openapi.yml
  format: yaml
  label: Howler Email OTP API
  slug: howler-email-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-email-otp-api-openapi.yml
- filename: howler-events-api-openapi.yml
  format: yaml
  label: Howler Events API
  slug: howler-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-events-api-openapi.yml
- filename: howler-oauth-api-openapi.yml
  format: yaml
  label: Howler OAuth API
  slug: howler-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-oauth-api-openapi.yml
- filename: howler-third-party-oauth-api-openapi.yml
  format: yaml
  label: Howler Third Party OAuth API
  slug: howler-third-party-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-third-party-oauth-api-openapi.yml
- filename: howler-tickets-api-openapi.yml
  format: yaml
  label: Howler Tickets API
  slug: howler-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-tickets-api-openapi.yml
- filename: howler-top-up-api-openapi.yml
  format: yaml
  label: Howler Top Up API
  slug: howler-top-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-api-openapi.yml
- filename: howler-top-up-cashless-tag-api-openapi.yml
  format: yaml
  label: Howler Top Up Cashless Tag API
  slug: howler-top-up-cashless-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-cashless-tag-api-openapi.yml
- filename: howler-top-up-ticket-api-openapi.yml
  format: yaml
  label: Howler Top Up Ticket API
  slug: howler-top-up-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-ticket-api-openapi.yml
- filename: howler-topupables-api-openapi.yml
  format: yaml
  label: Howler Topupables API
  slug: howler-topupables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-topupables-api-openapi.yml
- filename: howler-transfer-ticket-api-openapi.yml
  format: yaml
  label: Howler Transfer Ticket API
  slug: howler-transfer-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-transfer-ticket-api-openapi.yml
- filename: howler-user-api-openapi.yml
  format: yaml
  label: Howler User API
  slug: howler-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-user-api-openapi.yml
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
- Event
- Ticketing
- Payments
- Cashless
- RFID
- Event Management
- Fintech
- South Africa
---
