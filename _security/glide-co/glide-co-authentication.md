---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Glide partner API and MCP OAuth flow.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Glide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glide declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Glide
provider_slug: glide-co
scheme_count: 3
schemes:
- evidence: 'Authenticate with HTTP Basic: form-encode each credential, then base64-encode `client_id:client_secret` per RFC 6749 section 2.3.1.'
  how_to_obtain: A Glide admin creates your partner record and returns `client_id` and `client_secret` once.
  name: Partner token request
  token_url: https://glide.co/api/partner/oauth/token
  type: http-basic
- evidence: 'Send `Authorization: Bearer <access_token>` on every resource request.'
  header: Authorization
  how_to_obtain: Mint a token via the partner token endpoint using client credentials.
  location: header
  name: Partner API bearer token
  type: http-bearer
- authorize_url: https://auth.glide.co/oauth2/authorize
  evidence: End-to-end authorization_code + PKCE flow for MCP clients.
  how_to_obtain: Register dynamically at `https://auth.glide.co/oauth2/register` to receive `client_id` and `client_secret`.
  name: MCP authorization_code flow
  scopes:
  - accounts:read
  - payments:initiate
  - payments:simulate
  - audit:stream
  token_url: https://auth.glide.co/oauth2/token
  type: oauth2
slug: glide-co-authentication
source_filename: glide-co-authentication.yml
source_heading: Authentication Profile
source_url: https://glide.co/docs/partners/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://glide.co/docs/partners/authentication.md\nsources:\n- https://glide.co/docs/partners/authentication.md\n- https://glide.co/docs/oss/headless/oauth-flow.md\n- https://glide.co/docs/quickstart.md\n- https://glide.co/docs/agents/quickstart.md\ndescription: Authentication methods for Glide partner API and MCP OAuth flow.\nschemes:\n- type: http-basic\n  name: Partner token request\n  evidence: 'Authenticate with HTTP Basic: form-encode each credential, then base64-encode `client_id:client_secret` per RFC 6749 section 2.3.1.'\n  token_url: https://glide.co/api/partner/oauth/token\n  how_to_obtain: A Glide admin creates your partner record and returns `client_id` and `client_secret` once.\n- type: http-bearer\n  name: Partner API bearer token\n  evidence: 'Send `Authorization: Bearer <access_token>` on every resource request.'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Mint a token via the partner token endpoint using client credentials.\n- type: oauth2\n  name: MCP authorization_code flow\n  evidence: End-to-end authorization_code + PKCE flow for MCP clients.\n  token_url: https://auth.glide.co/oauth2/token\n  authorize_url: https://auth.glide.co/oauth2/authorize\n  scopes:\n  - accounts:read\n  - payments:initiate\n  - payments:simulate\n  - audit:stream\n  how_to_obtain: Register dynamically at `https://auth.glide.co/oauth2/register` to receive `client_id` and `client_secret`.\ndocs: https://glide.co/docs/partners/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/glide-co/authentication/glide-co-authentication.yml
summary_line: 3 schemes
tags:
- Fintech
- Banking
- Payments
- Global
---
