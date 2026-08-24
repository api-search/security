---
api_key_in:
- cookie
- header
api_specs:
- filename: guestready-rentalready-openapi.yml
  format: yaml
  label: RentalReady API
  slug: rentalready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/openapi/guestready-rentalready-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Guestready Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GuestReady secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GuestReady
provider_slug: guestready
scheme_count: 4
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/guestready-rentalready-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/guestready-rentalready-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    scopes: 52
    tokenUrl: /o/token/
  name: oauth2
  sources:
  - openapi/guestready-rentalready-openapi.yml
  type: oauth2
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/guestready-rentalready-openapi.yml
  type: apiKey
slug: guestready-authentication
source_filename: guestready-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: openapi/guestready-rentalready-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\n    scopes: 52\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/authentication/guestready-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Property Management
- Short Term Rentals
- Vacation Rentals
- Hospitality
- Travel
- Real Estate
- Channel Management
- Reservations
- Revenue Management
- PMS
- MCP
- OAuth
---
