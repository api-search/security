---
api_key_in:
- header
api_specs:
- filename: montran-global-payments-hub-openapi.yml
  format: yaml
  label: Montran Global Payments Hub
  slug: montran-global-payments-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-global-payments-hub-openapi.yml
- filename: montran-instant-payments-gateway-openapi.yml
  format: yaml
  label: Montran Instant Payments Gateway
  slug: montran-instant-payments-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-instant-payments-gateway-openapi.yml
- filename: montran-payments-connectivity-openapi.yml
  format: yaml
  label: Montran Payments Connectivity
  slug: montran-payments-connectivity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-payments-connectivity-openapi.yml
- filename: montran-corporate-payments-portal-openapi.yml
  format: yaml
  label: Montran Corporate Payments Portal
  slug: montran-corporate-payments-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-corporate-payments-portal-openapi.yml
- filename: montran-virtual-accounts-openapi.yml
  format: yaml
  label: Montran Virtual Accounts
  slug: montran-virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-virtual-accounts-openapi.yml
- filename: montran-sanctions-screening-openapi.yml
  format: yaml
  label: Montran Sanctions Screening
  slug: montran-sanctions-screening
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-sanctions-screening-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Montran Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Montran secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Montran
provider_slug: montran
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/montran-corporate-payments-portal-openapi.yml
  - openapi/montran-global-payments-hub-openapi.yml
  - openapi/montran-instant-payments-gateway-openapi.yml
  - openapi/montran-payments-connectivity-openapi.yml
  - openapi/montran-sanctions-screening-openapi.yml
  - openapi/montran-virtual-accounts-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/montran-corporate-payments-portal-openapi.yml
  - openapi/montran-global-payments-hub-openapi.yml
  - openapi/montran-payments-connectivity-openapi.yml
  - openapi/montran-sanctions-screening-openapi.yml
  - openapi/montran-virtual-accounts-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization for PSD2 AISP/PISP access
  flows:
  - authorizationUrl: https://auth.montran.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://auth.montran.com/oauth2/token
  name: oauth2
  sources:
  - openapi/montran-instant-payments-gateway-openapi.yml
  type: oauth2
slug: montran-authentication
source_filename: montran-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/montran-corporate-payments-portal-openapi.yml, openapi/montran-global-payments-hub-openapi.yml,\n  openapi/montran-instant-payments-gateway-openapi.yml, openapi/montran-payments-connectivity-openapi.yml,\n  openapi/montran-sanctions-screening-openapi.yml, openapi/montran-virtual-accounts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/montran-corporate-payments-portal-openapi.yml\n  - openapi/montran-global-payments-hub-openapi.yml\n  - openapi/montran-instant-payments-gateway-openapi.yml\n  - openapi/montran-payments-connectivity-openapi.yml\n  - openapi/montran-sanctions-screening-openapi.yml\n  - openapi/montran-virtual-accounts-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n \
  \ - openapi/montran-corporate-payments-portal-openapi.yml\n  - openapi/montran-global-payments-hub-openapi.yml\n  - openapi/montran-payments-connectivity-openapi.yml\n  - openapi/montran-sanctions-screening-openapi.yml\n  - openapi/montran-virtual-accounts-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.montran.com/oauth2/authorize\n    tokenUrl: https://auth.montran.com/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 authorization for PSD2 AISP/PISP access\n  sources:\n  - openapi/montran-instant-payments-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/authentication/montran-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
---
