---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Collimer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collimer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Collimer
provider_slug: collimer-com
scheme_count: 2
schemes:
- applies_to:
  - /api/v1
  - /api/v0
  description: 'API key created at /connect, sent as Authorization: Bearer <key>. Works for /api/v1 and /api/v0; "API keys cannot authenticate /mcp".'
  key_creation: https://app.collimer.com/connect
  name: ApiKey
  scheme: bearer
  type: http
- applies_to:
  - /mcp
  - /api/v1
  - /api/v0
  authorization_url: https://app.collimer.com/oauth/authorize
  bearer_methods:
  - header
  discovery:
  - https://app.collimer.com/.well-known/oauth-protected-resource
  - https://app.collimer.com/.well-known/oauth-authorization-server
  dynamic_client_registration: https://app.collimer.com/oauth/register
  flows:
  - authorization_code
  - refresh_token
  name: OAuth2
  pkce: S256
  refresh: 'Refresh tokens rotate: persist the new refresh token after every refresh; the old token cannot be used again. A refresh token expires after 90 days without use. Sharing one refresh token across runners can trigger reuse detection and revoke the grant.'
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  token_url: https://app.collimer.com/oauth/token
  type: oauth2
  version: OAuth 2.1
slug: collimer-com-authentication
source_filename: collimer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://app.collimer.com/docs\ndocs: https://app.collimer.com/docs\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: 'API key created at /connect, sent as Authorization: Bearer <key>. Works for /api/v1 and /api/v0; \"API keys cannot authenticate /mcp\".'\n  applies_to:\n  - /api/v1\n  - /api/v0\n  key_creation: https://app.collimer.com/connect\n- name: OAuth2\n  type: oauth2\n  version: OAuth 2.1\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  dynamic_client_registration: https://app.collimer.com/oauth/register\n  authorization_url: https://app.collimer.com/oauth/authorize\n  token_url: https://app.collimer.com/oauth/token\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  discovery:\n  - https://app.collimer.com/.well-known/oauth-protected-resource\n  - https://app.collimer.com/.well-known/oauth-authorization-server\n  bearer_methods:\n\
  \  - header\n  applies_to:\n  - /mcp\n  - /api/v1\n  - /api/v0\n  refresh: 'Refresh tokens rotate: persist the new refresh token after every refresh; the old token cannot be used again. A refresh token expires after 90 days without use. Sharing one refresh token across\n    runners can trigger reuse detection and revoke the grant.'\n"
source_yaml_url: https://artifacts.apis.io/collimer-com/authentication/collimer-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Visibility
- Generative Engine Optimization
- SEO
- Marketing
- Analytics
- AI Search
---
