---
api_key_in: []
api_specs:
- filename: twitter-x-x-api-v2-openapi.json
  format: json
  label: X API v2
  slug: x-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/openapi/twitter-x-x-api-v2-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Twitter X Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Twitter/X secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Twitter/X
provider_slug: twitter-x
scheme_count: 3
schemes:
- name: BearerToken
  scheme: bearer
  sources:
  - openapi/twitter-x-x-api-v2-openapi.json
  type: http
- flows:
  - authorizationUrl: https://api.x.com/2/oauth2/authorize
    flow: authorizationCode
    scopes: 21
    tokenUrl: https://api.x.com/2/oauth2/token
  name: OAuth2UserToken
  sources:
  - openapi/twitter-x-x-api-v2-openapi.json
  type: oauth2
- name: UserToken
  scheme: OAuth
  sources:
  - openapi/twitter-x-x-api-v2-openapi.json
  type: http
slug: twitter-x-authentication
source_filename: twitter-x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/twitter-x-x-api-v2-openapi.json\ndocs: https://docs.x.com/fundamentals/authentication/overview\nnotes: >-\n  Documented methods — OAuth 1.0a User Context (legacy, still supported for\n  user actions), App-only Bearer token (public data, app-level rate limits),\n  OAuth 2.0 Authorization Code with PKCE (user context with 21 fine-grained\n  scopes; see scopes/twitter-x-scopes.yml), and HTTP Basic auth on some\n  enterprise endpoints. Credentials come from the Developer Console\n  (console.x.com). The three OpenAPI securitySchemes below map to Bearer\n  (BearerToken), OAuth 2.0 user context (OAuth2UserToken), and OAuth 1.0a\n  (UserToken).\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- name: OAuth2UserToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://api.x.com/2/oauth2/authorize\n    tokenUrl: https://api.x.com/2/oauth2/token\n    scopes: 21\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- name: UserToken\n  type: http\n  scheme: OAuth\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/authentication/twitter-x-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Social
- Social Media
- Posts
- Real-Time
- Streaming
- News
- Developer Platform
---
