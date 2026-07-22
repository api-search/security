---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ring Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ring secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ring
provider_slug: ring
scheme_count: 1
schemes:
- description: 'All Ring Partner API requests require an OAuth 2.0 Bearer access token in the Authorization header (Authorization: Bearer <access_token>). Tokens are obtained through a one-way account-linking authorization-code flow with HMAC nonce verification. Access tokens are short-lived (expires_in 14400 seconds / 4 hours) and are renewed with the refresh token. All requests to the Amazon Vision API and the Ring OAuth server must be made server-to-server from the partner backend — browser-initiated requests are blocked by CORS.'
  flows:
  - flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    tokenUrl: https://oauth.ring.com/oauth/token
    token_lifetime_seconds: 14400
    token_type: Bearer
  name: OAuth2
  scheme: bearer
  sources:
  - https://developer.amazon.com/docs/ring/api-documentation.html
  type: oauth2
slug: ring-authentication
source_filename: ring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.amazon.com/docs/ring/api-documentation.html#authentication\ndocs: https://developer.amazon.com/docs/ring/api-documentation.html#token-exchange-flow\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  transport: Bearer token in Authorization header\n  account_linking: one-way (Ring user grants a partner app access)\n  server_to_server: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: bearer\n  description: >-\n    All Ring Partner API requests require an OAuth 2.0 Bearer access token in the\n    Authorization header (Authorization: Bearer <access_token>). Tokens are obtained through\n    a one-way account-linking authorization-code flow with HMAC nonce verification. Access\n    tokens are short-lived (expires_in 14400 seconds / 4 hours) and are renewed with the\n    refresh token. All requests to the Amazon Vision API and the Ring OAuth server must be\n    made server-to-server from\
  \ the partner backend — browser-initiated requests are blocked\n    by CORS.\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://oauth.ring.com/oauth/token\n    grant_types: [authorization_code, refresh_token]\n    token_lifetime_seconds: 14400\n    token_type: Bearer\n  sources:\n  - https://developer.amazon.com/docs/ring/api-documentation.html\nnotes: >-\n  Scopes are returned in the token response (scope field) but Ring does not publish an\n  enumerated scope reference; the granted scope is set by the partner app configuration in\n  the Ring Developer Console. Credentials (client_id / client_secret) are issued per\n  application in the Amazon Ring Developer Console.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ring/refs/heads/main/authentication/ring-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Home Security
- Smart Home
- IoT
- Video
- Cameras
- Doorbells
- Webhooks
- WebRTC
- Amazon
- Developer Platform
- MCP
---
