---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emdly-com-openapi-generated.yml
  format: yaml
  label: emdly API
  slug: emdly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emdly-com/openapi/_ae-authored/emdly-com-openapi-generated.yml
auth_types: []
description: Authentication for emdly MCP uses either OAuth 2.1 (authorization code flow) or a personal bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: emdly Authentication
name_suffix: Authentication
oauth_flows: []
overview: emdly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: emdly
provider_slug: emdly-com
scheme_count: 1
schemes:
- authorize_url: https://emdly.com/oauth/authorize
  evidence: Claude calls a tool that needs you (brain_*, submit_skill) → emdly answers 401 with OAuth discovery → Claude registers as an OAuth client and opens https://emdly.com/oauth/authorize → you sign in with Google or GitHub and approve the mcp:use scope → the browser sends Claude back with a code, Claude exchanges it for a token and retries the tool.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Sign in via the browser when a 401 with OAuth discovery is returned; approve the mcp:use scope to receive an access token.
  location: header
  name: OAuth
  scopes:
  - mcp:use
  type: http-bearer
slug: emdly-com-authentication
source_filename: emdly-com-authentication.yml
source_heading: Authentication Profile
source_url: https://emdly.com/docs.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://emdly.com/docs.md\nsources:\n- https://emdly.com/docs.md\ndescription: Authentication for emdly MCP uses either OAuth 2.1 (authorization code flow) or a personal bearer token.\nschemes:\n- type: http-bearer\n  name: OAuth\n  evidence: Claude calls a tool that needs you (brain_*, submit_skill) → emdly answers 401 with OAuth discovery → Claude registers as an OAuth\n    client and opens https://emdly.com/oauth/authorize → you sign in with Google or GitHub and approve the mcp:use scope → the browser sends Claude\n    back with a code, Claude exchanges it for a token and retries the tool.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://emdly.com/oauth/authorize\n  scopes:\n  - mcp:use\n  how_to_obtain: Sign in via the browser when a 401 with OAuth discovery is returned; approve the mcp:use scope to receive an access token.\n\
  docs: https://emdly.com/docs.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/emdly-com/authentication/emdly-com-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- Markdown skills
- Open Source
---
