---
anonymous_access: false
api_key_in: []
auth_types: []
description: OpenClaw Direct uses OAuth 2.0 Authorization Code flow with PKCE and also accepts user‑issued API tokens presented as Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OpenClaw Direct Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenClaw Direct declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenClaw Direct
provider_slug: openclaw-direct
scheme_count: 1
schemes:
- authorize_url: https://openclaw.direct/oauth/authorize
  evidence: 'The flow is: discover → register a client → get the user''s authorization → exchange the code for an access token → call the API → refresh or revoke.'
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register a public client via POST https://openclaw.direct/oauth/register (no client secret). Then direct the user to the authorize URL with response_type=code, client_id, redirect_uri, scope=mcp, code_challenge (PKCE S256), and state. After the user authorizes, exchange the code at the token endpoint using POST https://openclaw.direct/oauth/token with grant_type=authorization_code, code, redirect_uri, client_id, and code_verifier. Refresh tokens via the same token endpoint with grant_type=refresh_token.
  name: OAuth 2.0 Authorization Code with PKCE
  scopes:
  - mcp
  type: oauth2
slug: openclaw-direct-authentication
source_filename: openclaw-direct-authentication.yml
source_heading: Authentication Profile
source_url: https://openclaw.direct/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openclaw.direct/.well-known/oauth-authorization-server\nsources:\n- https://openclaw.direct/.well-known/oauth-authorization-server\n- https://openclaw.direct/.well-known/oauth-protected-resource\n- https://openclaw.direct/auth.md\n- https://openclaw.direct/blog/whatsapp-ban-openclaw-telegram-setup.md\ndescription: OpenClaw Direct uses OAuth 2.0 Authorization Code flow with PKCE and also accepts user‑issued API tokens presented as Bearer tokens.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Authorization Code with PKCE\n  evidence: 'The flow is: discover → register a client → get the user''s authorization → exchange the code for an access token → call the API\n    → refresh or revoke.'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://openclaw.direct/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: Register a public client via POST https://openclaw.direct/oauth/register\
  \ (no client secret). Then direct the user to the authorize\n    URL with response_type=code, client_id, redirect_uri, scope=mcp, code_challenge (PKCE S256), and state. After the user authorizes, exchange\n    the code at the token endpoint using POST https://openclaw.direct/oauth/token with grant_type=authorization_code, code, redirect_uri, client_id,\n    and code_verifier. Refresh tokens via the same token endpoint with grant_type=refresh_token.\ndocs: https://openclaw.direct/.well-known/oauth-authorization-server\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/openclaw-direct/authentication/openclaw-direct-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Managed Service
- OpenClaw
- Assistant
---
