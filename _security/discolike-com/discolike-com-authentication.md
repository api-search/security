---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DiscoLike Authentication
name_suffix: Authentication
oauth_flows: []
overview: DiscoLike declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DiscoLike
provider_slug: discolike-com
scheme_count: 2
schemes:
- evidence: 'Include your API key in the x-discolike-key header:'
  header: x-discolike-key
  how_to_obtain: Create and manage your keys at app.discolike.com/account/management/keys.
  location: header
  name: x-discolike-key
  type: apiKey
- authorize_url: https://auth.discolike.com/oauth/2.1/authorize?response_type=code&client_id=...
  evidence: Tokens are issued by the authorization server described at api.discolike.com/v1/.well-known/oauth-authorization-server, through the authorization-code flow with PKCE.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Run `discolike auth login` which opens the browser to the authorization URL, or register a public client dynamically as described in the docs.
  location: header
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - offline_access
  type: oauth2
slug: discolike-com-authentication
source_filename: discolike-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.discolike.com/cli/
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.discolike.com/cli/\nsources:\n- https://docs.discolike.com/cli/\n- https://docs.discolike.com/api/access/\n- https://docs.discolike.com/sdk/\n- https://docs.discolike.com/mcp/\nschemes:\n- type: apiKey\n  name: x-discolike-key\n  evidence: 'Include your API key in the x-discolike-key header:'\n  location: header\n  header: x-discolike-key\n  how_to_obtain: Create and manage your keys at app.discolike.com/account/management/keys.\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: Tokens are issued by the authorization server described at api.discolike.com/v1/.well-known/oauth-authorization-server, through the\n    authorization-code flow with PKCE.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://auth.discolike.com/oauth/2.1/authorize?response_type=code&client_id=...\n  scopes:\n  - offline_access\n\
  \  how_to_obtain: Run `discolike auth login` which opens the browser to the authorization URL, or register a public client dynamically as described\n    in the docs.\ndocs: https://docs.discolike.com/cli/\n"
source_yaml_url: https://artifacts.apis.io/discolike-com/authentication/discolike-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Market Intelligence
- Data Aggregation
- API Platform
- Competitive Analysis
---
