---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Giving Block Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Giving Block declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Giving Block
provider_slug: the-giving-block
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT access token obtained from POST /v1/login and refreshed via POST /v1/refresh-tokens. Sent as `Authorization: Bearer <accessToken>`.'
  id: bearerAuth
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: the-giving-block-authentication
source_filename: the-giving-block-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.thegivingblock.com/reference/getting-started-1 (Authentication Flow)\ndocs: https://docs.thegivingblock.com/docs/authentication-flow\napi: The Giving Block Public API\nsummary: >-\n  JWT-based, token authentication. Partners request API user credentials (and AES\n  encryption keys for webhook notifications) by emailing The Giving Block's integrations\n  team. Credentials are exchanged at the login endpoint for a short-lived access token\n  plus a refresh token; the access token is sent as a bearer token on every request and\n  renewed via the refresh-tokens endpoint. Server-to-server integration.\nschemes:\n- id: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  name: Authorization\n  description: >-\n    JWT access token obtained from POST /v1/login and refreshed via\n    POST /v1/refresh-tokens. Sent as `Authorization: Bearer <accessToken>`.\nflows:\n- name: login\n  operationId:\
  \ login\n  method: POST\n  path: /v1/login\n  description: Exchange issued API user credentials for an access token and refresh token.\n- name: refreshTokens\n  operationId: refreshTokens\n  method: POST\n  path: /v1/refresh-tokens\n  description: Exchange a valid refresh token for a new access token.\ncredentials:\n  provisioning: manual\n  how: Email the integrations team to request API user credentials and AES webhook keys.\n  environments:\n  - name: production\n    baseURL: https://public-api.tgbwidget.com\n  - name: sandbox\n    baseURL: https://public-api.sandbox.thegivingblock.com\nnotes:\n- No OAuth2 authorization/token URLs are published; auth is a custom JWT login exchange.\n- Webhook payloads are AES-256 encrypted using keys issued alongside API credentials.\n- Common auth error codes include INVALID_JWT_TOKEN.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-giving-block/refs/heads/main/authentication/the-giving-block-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Crypto Web3
- Donations
- Fundraising
- Non-Profit
- Payments
- Cryptocurrency
- Stock Donations
- Webhook
- Widgets
---
