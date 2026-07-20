---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flowdesk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flowdesk secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flowdesk
provider_slug: flowdesk
scheme_count: 2
schemes:
- bearer_format: JWT
  description: Requests to the Platform Connect REST API (api.flowdesk.co) and WebSocket channel (ws.flowdesk.co) are authorized with a JWT bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.flowdesk.co/getting-started/authentication
  type: http
- auth_domain: login.flowdesk.co
  description: OAuth 2.0 tokens are issued through Flowdesk's Auth0 tenant (login.flowdesk.co). The documentation includes a JWT generation reference (docs.flowdesk.co/reference/jwt-generate) for producing the bearer token presented to the API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.flowdesk.co/oauth/token
  name: oauth2
  provider: Auth0
  sources:
  - https://docs.flowdesk.co/reference/jwt-generate
  - https://docs.flowdesk.co/config.js
  type: oauth2
slug: flowdesk-authentication
source_filename: flowdesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.flowdesk.co/getting-started/authentication\nnotes: >-\n  Derived from Flowdesk Platform Connect developer documentation and the docs\n  site runtime config (docs.flowdesk.co/config.js), which declares the Auth0\n  tenant, API host, and WebSocket host. No downloadable OpenAPI document is\n  published by the docs site (the reference is rendered client-side in\n  Docusaurus), so scheme details below are captured from the published docs\n  surface rather than derived from a spec file.\nsummary:\n  types:\n  - oauth2\n  - http\n  bearer_format: JWT\n  oauth2_flows:\n  - clientCredentials\n  identity_provider: Auth0\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Requests to the Platform Connect REST API (api.flowdesk.co) and WebSocket\n    channel (ws.flowdesk.co) are authorized with a JWT bearer token in the\n    Authorization header.\n  sources:\n  - https://docs.flowdesk.co/getting-started/authentication\n\
  - name: oauth2\n  type: oauth2\n  provider: Auth0\n  auth_domain: login.flowdesk.co\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.flowdesk.co/oauth/token\n  description: >-\n    OAuth 2.0 tokens are issued through Flowdesk's Auth0 tenant\n    (login.flowdesk.co). The documentation includes a JWT generation reference\n    (docs.flowdesk.co/reference/jwt-generate) for producing the bearer token\n    presented to the API.\n  sources:\n  - https://docs.flowdesk.co/reference/jwt-generate\n  - https://docs.flowdesk.co/config.js\nhosts:\n  api: https://api.flowdesk.co\n  websocket: wss://ws.flowdesk.co\n  auth: https://login.flowdesk.co\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowdesk/refs/heads/main/authentication/flowdesk-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Fintech
- Crypto
- Digital Assets
- Trading
- Liquidity
- Market Maker
- OTC
- WebSocket
---
