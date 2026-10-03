---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Maxvideoai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MaxVideoAI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MaxVideoAI
provider_slug: maxvideoai
scheme_count: 1
schemes:
- authorization_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/authorize
  bearer_methods:
  - header
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.maxvideoai.com
  name: OAuth2
  pkce: S256
  registration_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/clients/register
  scopes:
  - openid
  - email
  - profile
  - offline_access
  sources:
  - well-known/maxvideoai-oauth-authorization-server.json
  - well-known/maxvideoai-oauth-protected-resource-mcp.json
  token_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: maxvideoai-authentication
source_filename: maxvideoai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: >-\n  https://api.maxvideoai.com/.well-known/oauth-authorization-server,\n  https://api.maxvideoai.com/.well-known/oauth-protected-resource/mcp,\n  https://maxvideoai.com/docs/mcp\nsummary:\n  types: [oauth2]\n  oauth2_version: '2.1'\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  notes: >-\n    Access to the MCP server is exclusively via OAuth 2.1 (authorization code +\n    PKCE). No API keys, bearer tokens, query params or passwords are appended to\n    the endpoint URL. There is no REST API and no customer API-key surface.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorization_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/authorize\n  token_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token\n  registration_endpoint: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/clients/register\n  issuer: https://api.maxvideoai.com\n  pkce: S256\n  dynamic_client_registration:\
  \ true\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  bearer_methods: [header]\n  scopes: [openid, email, profile, offline_access]\n  sources:\n  - well-known/maxvideoai-oauth-authorization-server.json\n  - well-known/maxvideoai-oauth-protected-resource-mcp.json\ndocs: https://maxvideoai.com/docs/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxvideoai/refs/heads/main/authentication/maxvideoai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Video Generation
- Image Generation
- MCP
- Agent-Native
- Text-to-Video
- Image-to-Video
- Creative Production
- Pay As You Go
---
