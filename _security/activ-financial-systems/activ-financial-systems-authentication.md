---
api_key_in: []
auth_types:
- credentials
description: ''
kind: authentication
layout: security
method: searched
name: Activ Financial Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACTIV Financial Systems secures its APIs with credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ACTIV Financial Systems
provider_slug: activ-financial-systems
scheme_count: 1
schemes:
- description: user + password supplied in ConnectParameters when calling connect() against a customer-provisioned OneApi Gateway host; session-scoped, one active session at a time.
  name: OneApiGatewayCredentials
  parameters:
  - description: The host to connect to (customer-provisioned OneApi Gateway).
    name: host
    required: false
  - description: The username to connect with.
    name: user
    required: false
  - description: The password for the user.
    name: password
    required: false
  sources:
  - https://weboneapi.activfinancial.com/documentation/session/connect
  - https://unpkg.com/@activfinancial/one-api@1.1.4/lib/docs.json
  type: credentials
slug: activ-financial-systems-authentication
source_filename: activ-financial-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://weboneapi.activfinancial.com/documentation/session/connect\ndocs: https://weboneapi.activfinancial.com/tutorials\nnote: The OnePlatform Web API (One API) is not a REST API and publishes no OpenAPI\n  securitySchemes; authentication is credential-based at WebSocket session connect.\n  The published ConnectParameters contract (session/connect) takes host, user, and\n  password; connect() establishes a session to a OneApi Gateway and rejects with\n  StatusCode values such as invalidUser, invalidPassword, accessDenied, and\n  notLicensed on failure. Gateway hosts and credentials are provisioned per customer\n  by ACTIV/Options Technology - there is no self-serve sign-up, OAuth, or API-key\n  scheme documented. Market data access is further entitled per user (permissionId,\n  notPermissioned status codes).\nsummary:\n  types:\n  - credentials\n  transport: websocket\n  oauth2_flows: []\n  api_key_in: []\n  self_serve_signup:\
  \ false\nschemes:\n- name: OneApiGatewayCredentials\n  type: credentials\n  description: user + password supplied in ConnectParameters when calling connect()\n    against a customer-provisioned OneApi Gateway host; session-scoped, one active\n    session at a time.\n  parameters:\n  - name: host\n    description: The host to connect to (customer-provisioned OneApi Gateway).\n    required: false\n  - name: user\n    description: The username to connect with.\n    required: false\n  - name: password\n    description: The password for the user.\n    required: false\n  sources:\n  - https://weboneapi.activfinancial.com/documentation/session/connect\n  - https://unpkg.com/@activfinancial/one-api@1.1.4/lib/docs.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activ-financial-systems/refs/heads/main/authentication/activ-financial-systems-authentication.yml
summary_line: credentials · 1 scheme
tags:
- Company
- Fintech
- Market Data
- Financial Data
- Real-Time Data
- Streaming
- WebSocket
- Trading Infrastructure
- Options Technology
---
