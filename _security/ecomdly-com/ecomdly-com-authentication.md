---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ecomdly-com-openapi-generated.yml
  format: yaml
  label: ecomdly API
  slug: ecomdly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomdly-com/openapi/_ae-authored/ecomdly-com-openapi-generated.yml
auth_types: []
description: Authentication methods for ecomdly MCP server
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ecomdly Authentication
name_suffix: Authentication
oauth_flows: []
overview: ecomdly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ecomdly
provider_slug: ecomdly-com
scheme_count: 1
schemes:
- authorize_url: https://ecomdly.com/oauth/authorize
  evidence: Claude calls a tool that needs you (brain_*, submit_skill) → ecomdly answers 401 with OAuth discovery → Claude registers as an OAuth client and opens https://ecomdly.com/oauth/authorize → you sign in with Google or GitHub and approve the `mcp:use` scope → the browser sends Claude back with a code, Claude exchanges it for a token and retries the tool.
  flows:
  - authorization_code
  how_to_obtain: Sign in with Google or GitHub via the OAuth authorization page and approve the `mcp:use` scope.
  name: OAuth 2.1 PKCE
  scopes:
  - mcp:use
  type: oauth2
slug: ecomdly-com-authentication
source_filename: ecomdly-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ecomdly.com/docs.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ecomdly.com/docs.md\nsources:\n- https://ecomdly.com/docs.md\ndescription: Authentication methods for ecomdly MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.1 PKCE\n  evidence: Claude calls a tool that needs you (brain_*, submit_skill) → ecomdly answers 401 with OAuth discovery → Claude registers as an OAuth\n    client and opens https://ecomdly.com/oauth/authorize → you sign in with Google or GitHub and approve the `mcp:use` scope → the browser sends\n    Claude back with a code, Claude exchanges it for a token and retries the tool.\n  flows:\n  - authorization_code\n  authorize_url: https://ecomdly.com/oauth/authorize\n  scopes:\n  - mcp:use\n  how_to_obtain: Sign in with Google or GitHub via the OAuth authorization page and approve the `mcp:use` scope.\ndocs: https://ecomdly.com/docs.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/ecomdly-com/authentication/ecomdly-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-Commerce
- Artificial Intelligence
- Agents
- Skills
- Integration
---
