---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Notice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notice declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Notice
provider_slug: notice
scheme_count: 3
schemes:
- applies_to: https://api.notice.co/mcp
  authorization_endpoint: https://notice.co/oauth/authorize
  challenge: 'WWW-Authenticate: Bearer resource_metadata="https://api.notice.co/.well-known/oauth-protected-resource"'
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: mcp_oauth2
  id_token_signing_alg_values_supported:
  - RS256
  identity_provider: Stytch (api.stytch.notice.co, a Notice-controlled subdomain)
  issuer: https://api.stytch.notice.co
  jwks_uri: https://api.stytch.notice.co/.well-known/jwks.json
  method: probed
  pkce: S256
  registration_endpoint: https://api.stytch.notice.co/v1/oauth2/register
  token_endpoint: https://api.stytch.notice.co/v1/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://api.stytch.notice.co/v1/oauth2/userinfo
- applies_to: https://api.notice.co/v1
  documented: false
  evidence:
  - body: '{"error":"Not authorized"}'
    http_status: 401
    probe: GET https://api.notice.co/v1/openapi.json
  - http_status: 401
    probe: GET https://api.notice.co/v1/
  id: rest_v1
  method: probed
  note: The help centre states the Notice API is RESTful and sold as an enterprise subscription, but names no credential type, header, or key prefix on any public page. No API-key scheme is asserted here because none is published - the honest reading is that the auth model is documented only to subscribers.
  type: unknown
- applies_to: https://api.notice.co
  attributes: secure; httponly; samesite=lax
  id: session_cookie
  method: probed
  name: _notice_session
  note: First-party browser session for notice.co; not an integration credential.
  type: cookie
slug: notice-authentication
source_filename: notice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://api.notice.co/.well-known/oauth-protected-resource\nalso_source:\n  - https://api.stytch.notice.co/.well-known/oauth-authorization-server\n  - https://api.stytch.notice.co/.well-known/openid-configuration\n  - https://learn.notice.co/en/articles/8422141-how-does-the-notice-api-work\nsummary: >-\n  Notice publishes no OpenAPI a machine can read (api.notice.co/v1/openapi.json exists but answers\n  401), so this profile is built from the two auth-discovery documents Notice actually serves plus\n  the observed challenge behaviour of the API and MCP endpoints. Two distinct surfaces:\n  a REST v1 API sold as an enterprise subscription, whose credential scheme is not documented\n  publicly, and an OAuth 2.1-style MCP endpoint whose entire handshake is discoverable anonymously.\nschemes:\n  - id: mcp_oauth2\n    type: oauth2\n    applies_to: https://api.notice.co/mcp\n    flow: authorizationCode\n    pkce: S256\n    issuer: https://api.stytch.notice.co\n\
  \    authorization_endpoint: https://notice.co/oauth/authorize\n    token_endpoint: https://api.stytch.notice.co/v1/oauth2/token\n    userinfo_endpoint: https://api.stytch.notice.co/v1/oauth2/userinfo\n    registration_endpoint: https://api.stytch.notice.co/v1/oauth2/register\n    jwks_uri: https://api.stytch.notice.co/.well-known/jwks.json\n    id_token_signing_alg_values_supported:\n      - RS256\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    identity_provider: Stytch (api.stytch.notice.co, a Notice-controlled subdomain)\n    challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://api.notice.co/.well-known/oauth-protected-resource\"'\n    method: probed\n  - id: rest_v1\n    type: unknown\n    applies_to: https://api.notice.co/v1\n    documented: false\n    evidence:\n  \
  \    - probe: GET https://api.notice.co/v1/openapi.json\n        http_status: 401\n        body: '{\"error\":\"Not authorized\"}'\n      - probe: GET https://api.notice.co/v1/\n        http_status: 401\n    note: >-\n      The help centre states the Notice API is RESTful and sold as an enterprise subscription, but\n      names no credential type, header, or key prefix on any public page. No API-key scheme is\n      asserted here because none is published - the honest reading is that the auth model is\n      documented only to subscribers.\n    method: probed\n  - id: session_cookie\n    type: cookie\n    applies_to: https://api.notice.co\n    name: _notice_session\n    attributes: 'secure; httponly; samesite=lax'\n    note: First-party browser session for notice.co; not an integration credential.\n    method: probed\nsession_headers_observed:\n  - 'access-control-expose-headers: X-Stytch-Session-JWT'\ndocs: null\ndocs_note: >-\n  No public authentication reference page exists. notice.co\
  \ returns HTTP 403 (Cloudflare bot\n  block) to non-browser clients, and the help centre article on the API does not describe the\n  credential scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notice/refs/heads/main/authentication/notice-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Private Markets
- Market Data
- Financial Data
- Investing
- Pre-IPO
- Secondary Markets
- Valuations
- Fintech
- MCP
---
