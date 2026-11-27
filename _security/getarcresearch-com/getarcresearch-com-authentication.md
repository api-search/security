---
anonymous_access: false
api_key_in: []
auth_types: []
description: Arc Research supports MCP OAuth and bearer‑token authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arc Research Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arc Research declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arc Research
provider_slug: getarcresearch-com
scheme_count: 1
schemes:
- authorize_url: https://www.getarcresearch.com/oauth/authorize
  evidence: Arc Research MCP supports MCP OAuth (what Claude.ai custom connectors expect) and personal bearer tokens for Cursor, Claude Code, and Perplexity.
  header: Authorization
  how_to_obtain: Register a client (POST https://www.getarcresearch.com/oauth/register or use a client_id metadata document), then send the user to the authorize URL with response_type=code, client_id, redirect_uri, scope=mcp, resource=https://www.getarcresearch.com/mcp, and PKCE. Exchange the code at the token endpoint to receive an access token. Refresh tokens via the token endpoint as needed.
  location: header
  name: MCP OAuth
  scopes:
  - mcp
  type: oauth2
slug: getarcresearch-com-authentication
source_filename: getarcresearch-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.getarcresearch.com/docs/mcp/authentication
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.getarcresearch.com/docs/mcp/authentication\nsources:\n- https://www.getarcresearch.com/docs/mcp/authentication\n- https://www.getarcresearch.com/auth.md\ndescription: Arc Research supports MCP OAuth and bearer‑token authentication.\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: Arc Research MCP supports MCP OAuth (what Claude.ai custom connectors expect) and personal bearer tokens for Cursor, Claude Code,\n    and Perplexity.\n  location: header\n  header: Authorization\n  authorize_url: https://www.getarcresearch.com/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: Register a client (POST https://www.getarcresearch.com/oauth/register or use a client_id metadata document), then send the user\n    to the authorize URL with response_type=code, client_id, redirect_uri, scope=mcp, resource=https://www.getarcresearch.com/mcp, and PKCE. Exchange\n    the code\
  \ at the token endpoint to receive an access token. Refresh tokens via the token endpoint as needed.\ndocs: https://www.getarcresearch.com/docs/mcp/authentication\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/getarcresearch-com/authentication/getarcresearch-com-authentication.yml
summary_line: 1 scheme
tags:
- Commodity
- Data
- Analytics
- Research
- Platform
---
