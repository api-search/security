---
anonymous_access: false
api_key_in: []
api_specs:
- filename: parse-gl-openapi-generated.yml
  format: yaml
  label: Parse API
  slug: parse-gl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parse-gl/openapi/_ae-authored/parse-gl-openapi-generated.yml
auth_types: []
description: Parse agents authenticate via OAuth sign‑in or by presenting a workspace key as a Bearer token.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Parse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parse declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Parse
provider_slug: parse-gl
scheme_count: 2
schemes:
- evidence: An MCP client that signs in with OAuth ... Sign in with Parse when the server asks (calling `get_brief` logged out answers 401 with the challenge)
  name: Parse OAuth
  type: oauth2
- evidence: '`Authorization: Bearer parse_mcp_…`'
  header: Authorization
  how_to_obtain: Created via `POST https://agent.parse.gl/v1/workspaces` (unclaimed) or `POST https://agent.parse.gl/v1/workspaces/claim` after claim, returning a key prefixed with `parse_mcp_` or `parse_uws_`.
  location: header
  name: Workspace key
  type: http-bearer
slug: parse-gl-authentication
source_filename: parse-gl-authentication.yml
source_heading: Authentication Profile
source_url: https://parse.gl/auth.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://parse.gl/auth.md\nsources:\n- https://parse.gl/auth.md\ndescription: Parse agents authenticate via OAuth sign‑in or by presenting a workspace key as a Bearer token.\nschemes:\n- type: oauth2\n  name: Parse OAuth\n  evidence: An MCP client that signs in with OAuth ... Sign in with Parse when the server asks (calling `get_brief` logged out answers 401 with\n    the challenge)\n- type: http-bearer\n  name: Workspace key\n  evidence: '`Authorization: Bearer parse_mcp_…`'\n  location: header\n  header: Authorization\n  how_to_obtain: Created via `POST https://agent.parse.gl/v1/workspaces` (unclaimed) or `POST https://agent.parse.gl/v1/workspaces/claim` after\n    claim, returning a key prefixed with `parse_mcp_` or `parse_uws_`.\ndocs: https://parse.gl/auth.md\n"
source_yaml_url: https://artifacts.apis.io/parse-gl/authentication/parse-gl-authentication.yml
summary_line: 2 schemes
tags:
- AI Visibility
- Market Research
- Citation Tracking
- AI Agents
- Pricing
---
