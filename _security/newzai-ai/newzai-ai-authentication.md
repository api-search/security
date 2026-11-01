---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for NewzAI MCP as described on the provider page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Newzai Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: newzai-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: newzai-ai
provider_slug: newzai-ai
scheme_count: 1
schemes:
- authorize_url: https://api.newzai.ai/authorize
  evidence: OAuth 2.0 was the obvious choice. It's the standard MCP clients expect, it gives us scoped access, token expiry, and a proper refresh cycle.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Client registers via POST /register to receive client_id and client_secret, then performs the OAuth authorization code flow using PKCE.
  name: OAuth2
  scopes:
  - openid
  - https://www.googleapis.com/auth/userinfo.email
  - https://www.googleapis.com/auth/userinfo.profile
  type: oauth2
slug: newzai-ai-authentication
source_filename: newzai-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://newzai.ai/resources/blogs/mcp-oauth-implementation
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://newzai.ai/resources/blogs/mcp-oauth-implementation\nsources:\n- https://newzai.ai/resources/blogs/mcp-oauth-implementation\ndescription: Authentication methods for NewzAI MCP as described on the provider page.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: OAuth 2.0 was the obvious choice. It's the standard MCP clients expect, it gives us scoped access, token expiry, and a proper refresh\n    cycle.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://api.newzai.ai/authorize\n  scopes:\n  - openid\n  - https://www.googleapis.com/auth/userinfo.email\n  - https://www.googleapis.com/auth/userinfo.profile\n  how_to_obtain: Client registers via POST /register to receive client_id and client_secret, then performs the OAuth authorization code flow using\n    PKCE.\ndocs: https://newzai.ai/resources/blogs/mcp-oauth-implementation\nnote: 1 extracted\
  \ row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/newzai-ai/authentication/newzai-ai-authentication.yml
summary_line: 1 scheme
tags:
- News
- AI
- Aggregation
- Personalization
- Multilingual
---
