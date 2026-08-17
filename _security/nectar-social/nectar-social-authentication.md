---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Nectar Social Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nectar Social secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nectar Social
provider_slug: nectar-social
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://beta-api.nectarsocial.com/oauth/authorize
    flow: authorizationCode
    scope_count: 18
    scopes: scopes/nectar-social-scopes.yml
    tokenUrl: https://beta-api.nectarsocial.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://beta-api.nectarsocial.com
  name: OAuth2
  registration_endpoint: https://beta-api.nectarsocial.com/oauth/register
  resource_indicators_supported: true
  response_modes_supported:
  - query
  response_types_supported:
  - code
  revocation_endpoint: https://beta-api.nectarsocial.com/oauth/revoke
  revocation_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  sources:
  - https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: nectar-social-authentication
source_filename: nectar-social-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\nraw: well-known/nectar-social-oauth-authorization-server.json\nnote: >-\n  Nectar Social publishes no public OpenAPI, so this profile is built from the provider's own\n  RFC 8414 authorization server metadata and RFC 9728 protected resource metadata plus the\n  observed 401 challenges on the live API and MCP hosts. All values are transcribed from those\n  documents; nothing is inferred.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_token: true\n  pkce: S256\n  dynamic_client_registration: true\n  public_clients_supported: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://beta-api.nectarsocial.com\n  sources:\n  - https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://beta-api.nectarsocial.com/oauth/authorize\n\
  \    tokenUrl: https://beta-api.nectarsocial.com/oauth/token\n    scope_count: 18\n    scopes: scopes/nectar-social-scopes.yml\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  response_modes_supported: [query]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n  revocation_endpoint: https://beta-api.nectarsocial.com/oauth/revoke\n  revocation_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n  registration_endpoint: https://beta-api.nectarsocial.com/oauth/register\n  resource_indicators_supported: true\nprotected_resources:\n- resource: https://mcp.nectarsocial.com/mcp\n  kind: MCP server\n  authorization_servers: [https://beta-api.nectarsocial.com]\n  bearer_methods_supported: [header]\n  scopes_supported: [content:read, analytics:read]\n  challenge: >-\n    WWW-Authenticate: Bearer resource_metadata=\"https://mcp.nectarsocial.com/.well-known/oauth-protected-resource/mcp\"\
  \n- resource: https://beta-api.nectarsocial.com\n  kind: REST API (beta)\n  observed_401_body: >-\n    {\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Missing or invalid Bearer token.\"},\n    \"meta\":{\"request_id\":\"…\",\"timestamp\":\"…\"}}\n  note: every probed path on this host returns 401 until a Bearer token is presented\nposture:\n  strengths:\n  - Authorization-code flow with PKCE S256 mandated (no implicit, no password grant).\n  - Refresh tokens supported; a token revocation endpoint (RFC 7009) is published.\n  - Dynamic client registration (RFC 7591) is open, so an MCP client can self-register.\n  - token_endpoint_auth_methods_supported includes \"none\", so public/native clients are first class.\n  - resource_indicators_supported (RFC 8707) — tokens can be audience-bound to a specific resource.\n  - Scope vocabulary is fine-grained (resource:action across 18 scopes).\n  gaps:\n  - No OpenID Connect discovery document (/.well-known/openid-configuration returns 404) —\
  \ OAuth only, no identity layer advertised.\n  - No jwks_uri published in the authorization server metadata, so token signature verification keys are not discoverable.\n  - No public human documentation of the auth flow; docs.nectarsocial.com redirects into a login-gated app.\ndocs: null\nx-evidence:\n- url: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://mcp.nectarsocial.com/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://beta-api.nectarsocial.com/.well-known/openid-configuration\n  http_status: 404\n- url: https://mcp.nectarsocial.com/mcp\n  http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-social/refs/heads/main/authentication/nectar-social-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- AI
- Social Media
- Community Management
- Social Listening
- Influencer Marketing
- Customer Engagement
- Social Commerce
- MCP
- Agents
- OAuth
---
