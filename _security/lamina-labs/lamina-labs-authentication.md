---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lamina Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lamina Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lamina Labs
provider_slug: lamina-labs
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://api.laminalabs.ai/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://api.laminalabs.ai/oauth/register
    scopes:
      jobs:create: Submit Simi video generation jobs.
      jobs:read: Read Simi video job status and retrieve playback/download URLs.
    tokenUrl: https://api.laminalabs.ai/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://api.laminalabs.ai
  name: LaminaOAuth
  response_types_supported:
  - code
  sources:
  - well-known/lamina-labs-oauth-authorization-server.json
  - well-known/lamina-labs-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: lamina-labs-authentication
source_filename: lamina-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.laminalabs.ai/.well-known/oauth-authorization-server\ndocs: https://app.laminalabs.ai/simi\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  refresh: true\n  pkce_required_methods: [S256]\n  dynamic_client_registration: true\n  public_clients_supported: true\nschemes:\n- name: LaminaOAuth\n  type: oauth2\n  sources: [well-known/lamina-labs-oauth-authorization-server.json, well-known/lamina-labs-openid-configuration.json]\n  issuer: https://api.laminalabs.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.laminalabs.ai/oauth/authorize\n    tokenUrl: https://api.laminalabs.ai/oauth/token\n    registrationUrl: https://api.laminalabs.ai/oauth/register\n    scopes:\n      jobs:create: Submit Simi video generation jobs.\n      jobs:read: Read Simi video job status and retrieve playback/download URLs.\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code,\
  \ refresh_token]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\ntransport:\n  header: Authorization\n  scheme: Bearer\n  observed_unauthenticated_response:\n    status: 401\n    body: '{\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Missing credentials\"}}'\nnotes:\n- Support for the `none` token endpoint auth method plus mandatory PKCE (S256) and an\n  open dynamic client registration endpoint is the MCP remote-server authorization\n  profile, letting an agent register itself as a public client without a pre-issued\n  client secret.\n- No API-key scheme was observed; every unauthenticated request to the API host returns\n  the same UNAUTHORIZED envelope.\n- The MCP `initialize` and `tools/list` methods answer without credentials; tool\n  invocation requires a bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamina-labs/refs/heads/main/authentication/lamina-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Machine Learning
- Education
- Media
- Model Context Protocol
- Content Generation
---
