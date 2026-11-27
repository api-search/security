---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aiseotracker-openapi-generated.yml
  format: yaml
  label: AI SEO Tracker API
  slug: aiseotracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiseotracker/openapi/_ae-authored/aiseotracker-openapi-generated.yml
auth_types: []
description: OAuth authentication for MCP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AI SEO Tracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI SEO Tracker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AI SEO Tracker
provider_slug: aiseotracker
scheme_count: 1
schemes:
- evidence: Auth Sign in with OAuth Copy for LLM AI SEO Tracker MCP is an OAuth resource . The authorization server is Better Auth at /api/auth . Clients discover metadata at /.well-known/oauth-protected-resource/api/agent/mcp .
  flows:
  - authorization_code
  how_to_obtain: Client initiates an authorization code flow with PKCE in a browser, signs in, and allows access; the server then returns a Bearer token.
  name: OAuth
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
slug: aiseotracker-authentication
source_filename: aiseotracker-authentication.yml
source_heading: Authentication Profile
source_url: https://aiseotracker.com/docs/auth
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aiseotracker.com/docs/auth\nsources:\n- https://aiseotracker.com/docs/auth\n- https://aiseotracker.com/docs/setup-skill\n- https://aiseotracker.com/SKILL.md\ndescription: OAuth authentication for MCP\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Auth Sign in with OAuth Copy for LLM AI SEO Tracker MCP is an OAuth resource . The authorization server is Better Auth at /api/auth\n    . Clients discover metadata at /.well-known/oauth-protected-resource/api/agent/mcp .\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  how_to_obtain: Client initiates an authorization code flow with PKCE in a browser, signs in, and allows access; the server then returns a Bearer\n    token.\ndocs: https://aiseotracker.com/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/aiseotracker/authentication/aiseotracker-authentication.yml
summary_line: 1 scheme
tags:
- AI SEO
- LLM Rank Tracker
- SEO Tools
- AI Visibility
---
