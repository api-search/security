---
api_key_in: []
auth_types:
- oauth2
- http
description: 'Authentication profile derived from Zatanna''s live RFC 8414 OAuth 2.0 authorization-server metadata (https://api.zatanna.ai/.well-known/oauth-authorization-server) and RFC 9728 protected-resource metadata. No first-party OpenAPI is published, so this is drawn directly from the discovery documents. Two credential paths are observed: OAuth 2.0 Authorization Code + PKCE (for MCP / agent clients) and a Zatanna-issued API key (Bearer), which the /mcp 401 body explicitly requests ("Valid API key required").'
kind: authentication
layout: security
method: searched
name: Zatanna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zatanna secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zatanna
provider_slug: zatanna
scheme_count: 2
schemes:
- authorizationUrl: https://api.zatanna.ai/api/auth/mcp/authorize
  description: OAuth 2.0 Authorization Code with PKCE (S256), Dynamic Client Registration (RFC 7591) enabled. Issues RS256-signed ID tokens; supports refresh tokens via the offline_access scope. This is the MCP authorization surface.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg: RS256
  jwksUrl: https://api.zatanna.ai/api/auth/mcp/jwks
  name: zatannaOAuth
  pkce: S256
  registrationUrl: https://api.zatanna.ai/api/auth/mcp/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  source: https://api.zatanna.ai/.well-known/oauth-authorization-server
  tokenUrl: https://api.zatanna.ai/api/auth/mcp/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfoUrl: https://api.zatanna.ai/api/auth/mcp/userinfo
- description: Zatanna-issued API key presented as a Bearer token in the Authorization header. Observed from the /mcp endpoint's 401 response body ("Valid API key required") as an alternative to interactive OAuth.
  name: zatannaApiKey
  scheme: bearer
  source: https://api.zatanna.ai/mcp
  type: http
slug: zatanna-authentication
source_filename: zatanna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.zatanna.ai/.well-known/oauth-authorization-server\ndescription: >-\n  Authentication profile derived from Zatanna's live RFC 8414 OAuth 2.0\n  authorization-server metadata (https://api.zatanna.ai/.well-known/oauth-authorization-server)\n  and RFC 9728 protected-resource metadata. No first-party OpenAPI is published,\n  so this is drawn directly from the discovery documents. Two credential paths\n  are observed: OAuth 2.0 Authorization Code + PKCE (for MCP / agent clients)\n  and a Zatanna-issued API key (Bearer), which the /mcp 401 body explicitly\n  requests (\"Valid API key required\").\nsummary:\n  types:\n  - oauth2\n  - http\nschemes:\n- name: zatannaOAuth\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.zatanna.ai/api/auth/mcp/authorize\n  tokenUrl: https://api.zatanna.ai/api/auth/mcp/token\n  userinfoUrl: https://api.zatanna.ai/api/auth/mcp/userinfo\n  jwksUrl: https://api.zatanna.ai/api/auth/mcp/jwks\n\
  \  registrationUrl: https://api.zatanna.ai/api/auth/mcp/register\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  id_token_signing_alg: RS256\n  scopes: [openid, profile, email, offline_access]\n  description: >-\n    OAuth 2.0 Authorization Code with PKCE (S256), Dynamic Client Registration\n    (RFC 7591) enabled. Issues RS256-signed ID tokens; supports refresh tokens\n    via the offline_access scope. This is the MCP authorization surface.\n  source: https://api.zatanna.ai/.well-known/oauth-authorization-server\n- name: zatannaApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Zatanna-issued API key presented as a Bearer token in the Authorization\n    header. Observed from the /mcp endpoint's 401 response body\n    (\"Valid API key required\") as an alternative to interactive OAuth.\n  source: https://api.zatanna.ai/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zatanna/refs/heads/main/authentication/zatanna-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- API
- MCP
- AI Agents
- Integration
- Reverse Engineering
- Automation
- OAuth
- Y Combinator
---
