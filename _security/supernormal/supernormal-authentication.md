---
api_key_in:
- header
api_specs:
- filename: supernormal-openapi-original.json
  format: json
  label: Supernormal API
  slug: supernormal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/openapi/supernormal-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Supernormal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: supernormal secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: supernormal
provider_slug: supernormal
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-TOKEN
  sources:
  - openapi/supernormal-openapi-original.json
  type: apiKey
- flows:
  - authorizationUrl: https://api.supernormal.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://api.supernormal.com/oauth/register
    revocationUrl: https://api.supernormal.com/oauth/revoke
    tokenUrl: https://api.supernormal.com/oauth/token
  name: OAuth2
  sources:
  - well-known/supernormal-oauth-authorization-server.json
  type: oauth2
slug: supernormal-authentication
source_filename: supernormal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/supernormal-openapi-original.json\ndocs: https://docs.supernormal.com/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  The documented REST API (api.supernormal.com/api/v1) authenticates with a scoped API key\n  passed in the X-API-TOKEN header; keys are created in account settings\n  (https://app.supernormal.com/settings) and scoped to the minimum permissions needed.\n  Separately, Supernormal runs a full OAuth 2.0 authorization server (RFC 8414 metadata at\n  /.well-known/oauth-authorization-server) with authorization-code grant, refresh tokens,\n  PKCE (S256), and RFC 7591 dynamic client registration — used to authorize the OAuth-protected\n  MCP server (bearer token). The OAuth server advertises a different scope set\n  (recordings:read, projects:read, projects:write) than the API-key x-scopes.\nschemes:\n- name:\
  \ ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  sources:\n  - openapi/supernormal-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.supernormal.com/oauth/authorize\n    tokenUrl: https://api.supernormal.com/oauth/token\n    revocationUrl: https://api.supernormal.com/oauth/revoke\n    registrationUrl: https://api.supernormal.com/oauth/register\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n  sources:\n  - well-known/supernormal-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/authentication/supernormal-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Meetings
- Meeting Notes
- Transcription
- AI Agents
- Voice Agents
- Productivity
- Collaboration
- Model Context Protocol
- REST API
---
