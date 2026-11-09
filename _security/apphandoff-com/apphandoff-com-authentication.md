---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for AppHandoff as described in the documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apphandoff Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppHandoff declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AppHandoff
provider_slug: apphandoff-com
scheme_count: 3
schemes:
- evidence: 'Use token as Authorization: Bearer <token> for API calls from your app.'
  header: Authorization
  how_to_obtain: Obtain via email+password login (POST /api/auth/login) or magic link flow, which returns an access token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: cookieAuth
  how_to_obtain: Login via portal (email+password, magic link, or GitHub OAuth) sets a Supabase session cookie (sb-access-token).
  location: cookie
  name: Supabase session cookie
  type: apiKey
- authorize_url: /oauth/authorize
  evidence: MCP clients must use OAuth.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Use the authorization endpoint proxy (GET /oauth/authorize) to obtain an authorization code, then exchange it at the token endpoint (POST /api/oauth/token). Refresh tokens via POST /api/oauth/token with grant_type=refresh_token.
  name: MCP OAuth
  type: oauth2
slug: apphandoff-com-authentication
source_filename: apphandoff-com-authentication.yml
source_heading: Authentication Profile
source_url: https://apphandoff.com/docs/getting-started/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apphandoff.com/docs/getting-started/authentication\nsources:\n- https://apphandoff.com/docs/getting-started/authentication\n- https://apphandoff.com/docs/api/operations/getauthstatus\n- https://apphandoff.com/docs/api/operations/githuboauth\n- https://apphandoff.com/docs/api/operations/oauthauthorizeproxy\ndescription: Authentication methods for AppHandoff as described in the documentation.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Use token as Authorization: Bearer <token> for API calls from your app.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via email+password login (POST /api/auth/login) or magic link flow, which returns an access token.\n- type: apiKey\n  name: Supabase session cookie\n  evidence: cookieAuth\n  location: cookie\n  how_to_obtain: Login via portal (email+password, magic link, or GitHub OAuth) sets a\
  \ Supabase session cookie (sb-access-token).\n- type: oauth2\n  name: MCP OAuth\n  evidence: MCP clients must use OAuth.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: /oauth/authorize\n  how_to_obtain: Use the authorization endpoint proxy (GET /oauth/authorize) to obtain an authorization code, then exchange it at the token endpoint\n    (POST /api/oauth/token). Refresh tokens via POST /api/oauth/token with grant_type=refresh_token.\ndocs: https://apphandoff.com/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/apphandoff-com/authentication/apphandoff-com-authentication.yml
summary_line: 3 schemes
tags:
- AI Agents
- Coding Tools
- Agent Orchestration
- Multi‑Agent Coordination
---
