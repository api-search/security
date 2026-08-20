---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Akia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Akia secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Akia
provider_slug: akia
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://sys.akia.com/oauth/authorize
    flow: authorizationCode
    parameters:
    - client_id
    - scope
    - response_type=code
    - redirect_uri
    scope_count: 16
    scopes_source: scopes/akia-scopes.yml
    tokenUrl: https://api.akia.com/oauth/token
  - flow: refreshToken
    parameters:
    - refresh_token
    - grant_type=refresh_token
    - client_id
    - client_secret
    tokenUrl: https://api.akia.com/oauth/token
  name: OAuth2
  sources:
  - https://api.akia.com/docs/authentication
  spec: RFC 6749
  type: oauth2
- authorization_endpoint: https://sys.akia.ai/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://sys.akia.ai/
  name: OAuth2 (authorization-server metadata)
  registration_endpoint: https://sys.akia.ai/oauth/register
  response_types_supported:
  - code
  sources:
  - well-known/akia-oauth-authorization-server.json
  spec: RFC 8414
  token_endpoint: https://sys.akia.ai/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
- authorization_servers:
  - https://sys.akia.ai/
  name: Bearer (MCP resource)
  resource: https://sys.akia.ai/mcp
  scheme: bearer
  sources:
  - well-known/akia-oauth-protected-resource.json
  spec: RFC 9728
  type: http
slug: akia-authentication
source_filename: akia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://api.akia.com/docs/authentication\ndocs: https://api.akia.com/docs/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  bearer_token: true\n  api_key_in: []\n  note: 'Akia publishes no API-key path. Every documented REST operation requires an\n    OAuth 2.0 access token, and the MCP endpoint requires a Bearer token from the\n    same authorization server.'\nschemes:\n- name: OAuth2\n  type: oauth2\n  spec: RFC 6749\n  sources:\n  - https://api.akia.com/docs/authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sys.akia.com/oauth/authorize\n    tokenUrl: https://api.akia.com/oauth/token\n    parameters:\n    - client_id\n    - scope\n    - response_type=code\n    - redirect_uri\n    scope_count: 16\n    scopes_source: scopes/akia-scopes.yml\n  - flow: refreshToken\n    tokenUrl: https://api.akia.com/oauth/token\n    parameters:\n   \
  \ - refresh_token\n    - grant_type=refresh_token\n    - client_id\n    - client_secret\n- name: OAuth2 (authorization-server metadata)\n  type: oauth2\n  spec: RFC 8414\n  sources:\n  - well-known/akia-oauth-authorization-server.json\n  issuer: https://sys.akia.ai/\n  authorization_endpoint: https://sys.akia.ai/oauth/authorize\n  token_endpoint: https://sys.akia.ai/oauth/token\n  registration_endpoint: https://sys.akia.ai/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\n- name: Bearer (MCP resource)\n  type: http\n  scheme: bearer\n  spec: RFC 9728\n  sources:\n  - well-known/akia-oauth-protected-resource.json\n  resource: https://sys.akia.ai/mcp\n  authorization_servers:\n  - https://sys.akia.ai/\ntoken_lifetimes:\n  authorization_code: 10 minutes, single use\n  access_token: 24 hours (expires_in\
  \ 86400)\n  refresh_token: 'single use — expires together with the previous access token once\n    exchanged'\nredirect_uri_rules:\n- Must use HTTPS\n- Must not contain a fragment (#)\n- 'When supplied at the authorize step it must be repeated verbatim at the token\n  exchange'\nguidance:\n  from_docs: 'Even though it can be done, you should not refresh the token on every\n    call. This API call is very expensive and will cause your system to be rate\n    limited quickly.'\naccess_model:\n  onboarding: request\n  note: 'Access to Akia''s API is currently available to select partners. Requests go\n    to partnerships@akia.com.'\nx-evidence:\n  fetched: '2026-08-06'\n  urls:\n  - url: https://api.akia.com/docs/authentication\n    http_status: 200\n  - url: https://api.akia.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.akia.com/.well-known/oauth-protected-resource\n    http_status: 200\n  note: 'Derived nothing from OpenAPI — Akia publishes no machine-readable\
  \ spec. Every\n    field above is transcribed from the provider''s own docs or its well-known\n    metadata documents.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akia/refs/heads/main/authentication/akia-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Hospitality
- Hotels
- Vacation Rentals
- Guest Experience
- Messaging
- Artificial Intelligence
- Agents
- Property Management
- Check-in
---
