---
api_key_in: []
api_specs:
- filename: streamelements-openapi-original.yml
  format: yaml
  label: StreamElements API
  slug: streamelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/openapi/streamelements-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Streamelements Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: StreamElements secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: StreamElements
provider_slug: streamelements
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: JWTBearer
  scheme: bearer
  sources:
  - openapi/streamelements-openapi-original.yml
  type: http
- flows:
  - authorizationUrl: https://api.streamelements.com/oauth2/authorize
    flow: authorizationCode
    scopes: 17
    tokenUrl: https://api.streamelements.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/streamelements-openapi-original.yml
  type: oauth2
slug: streamelements-authentication
source_filename: streamelements-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/streamelements-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: JWTBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.streamelements.com/oauth2/authorize\n    tokenUrl: https://api.streamelements.com/oauth2/token\n    scopes: 17\n  sources:\n  - openapi/streamelements-openapi-original.yml\ndocs: https://dev.streamelements.com/docs/api-docs/authentication\nnote: 'Three token types: channel JWT (personal access), overlay API key, and OAuth2 authorization-code\n  access tokens. JWT and overlay key are copied from the dashboard (Show Secrets); OAuth2 endpoints: /oauth2/authorize,\n  /oauth2/token, /oauth2/revoke.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/authentication/streamelements-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Live Streaming
- Creator Economy
- Overlays
- Chatbot
- Monetization
- Donations
- Loyalty Points
- Giveaways
- Video
- Twitch
- YouTube
- Real-Time
- WebSockets
- Webhooks
- REST
---
