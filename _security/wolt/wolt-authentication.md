---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wolt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Wolt secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Wolt
provider_slug: wolt
scheme_count: 2
schemes:
- flows:
  - client_auth: basic
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    scopes:
    - offline
    tokenUrl: https://integrations-authentication-service.wolt.com/oauth2/token
    tokenUrl_dev: https://integrations-authentication-service.development.dev.woltapi.com/oauth2/token
  name: OAuth2
  source: https://developer.wolt.com/docs/authentication20
  type: oauth2
- applies_to:
  - Order API
  - Wolt Drive API
  bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  source: https://developer.wolt.com/docs/api
  type: http
slug: wolt-authentication
source_filename: wolt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wolt.com/docs/authentication20\ndocs: https://developer.wolt.com/docs/authentication20\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken]\n  token_type: bearer\n  token_format: JWT\nnotes: >-\n  Wolt uses OAuth 2.0. The token endpoint is called with HTTP Basic authentication\n  (base64 of client_id:client_secret) and Content-Type application/x-www-form-urlencoded.\n  Access tokens are bearer JWTs valid for one hour; refresh tokens are single-use and\n  valid for 30 days (each refresh returns a new refresh token that must be cached).\n  API requests carry Authorization: Bearer {access_token}. Credentials are issued by a\n  Wolt account/technical account manager. Wolt Drive uses a Merchant Key bearer token.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://developer.wolt.com/docs/authentication20\n  flows:\n  - flow: authorizationCode\n    tokenUrl:\
  \ https://integrations-authentication-service.wolt.com/oauth2/token\n    tokenUrl_dev: https://integrations-authentication-service.development.dev.woltapi.com/oauth2/token\n    grant_types: [authorization_code, refresh_token]\n    scopes: [offline]\n    client_auth: basic\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  source: https://developer.wolt.com/docs/api\n  applies_to: [Order API, Wolt Drive API]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolt/refs/heads/main/authentication/wolt-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Marketplace
- Food Delivery
- Last Mile Delivery
- Logistics
- Webhooks
- OAuth
- Point of Sale
---
