---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for note1.ai
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: note1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: note1 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: note1
provider_slug: note1-ai
scheme_count: 2
schemes:
- authorize_url: https://api.note1.ai/oauth/authorize
  evidence: Authorization code flow with PKCE (S256 required) at `https://api.note1.ai/oauth/authorize`. The user approves access on the note1 consent page.
  flows:
  - authorization_code
  how_to_obtain: Register a client via `POST https://api.note1.ai/oauth/register` with redirect_uris; then perform the authorization code flow with PKCE.
  name: OAuth 2.1
  scopes:
  - meetings:read
  - calendar:read
  - meetings:write
  - integrations:write
  type: http-bearer
- evidence: A note1 user can create a token (prefix `n1_`) at https://note1.ai/dashboard/account/tokens and hand it to their agent.
  how_to_obtain: Create a token in the note1 dashboard under Account → Tokens.
  name: Personal access token
  type: http-bearer
slug: note1-ai-authentication
source_filename: note1-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://note1.ai/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://note1.ai/auth.md\nsources:\n- https://note1.ai/auth.md\ndescription: Authentication methods for note1.ai\nschemes:\n- type: http-bearer\n  name: OAuth 2.1\n  evidence: Authorization code flow with PKCE (S256 required) at `https://api.note1.ai/oauth/authorize`. The user approves access on the note1\n    consent page.\n  flows:\n  - authorization_code\n  authorize_url: https://api.note1.ai/oauth/authorize\n  scopes:\n  - meetings:read\n  - calendar:read\n  - meetings:write\n  - integrations:write\n  how_to_obtain: Register a client via `POST https://api.note1.ai/oauth/register` with redirect_uris; then perform the authorization code flow\n    with PKCE.\n- type: http-bearer\n  name: Personal access token\n  evidence: A note1 user can create a token (prefix `n1_`) at https://note1.ai/dashboard/account/tokens and hand it to their agent.\n  how_to_obtain: Create a token in the\
  \ note1 dashboard under Account → Tokens.\nnote: Both schemes send the token as a Bearer token in the `Authorization` header.\ndocs: https://note1.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/note1-ai/authentication/note1-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Note Taking
- Meeting Assistant
- Integration
- Productivity
---
