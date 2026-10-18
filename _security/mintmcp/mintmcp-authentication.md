---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mintmcp-openapi-generated.yml
  format: yaml
  label: MintMCP API
  slug: mintmcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintmcp/refs/heads/main/openapi/_ae-authored/mintmcp-openapi-generated.yml
auth_types: []
description: Client authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mintmcp Authentication
name_suffix: Authentication
oauth_flows: []
overview: MintMCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MintMCP
provider_slug: mintmcp
scheme_count: 1
schemes:
- evidence: Every MCP server exposes an OAuth 2.0 endpoint. AI clients use this to get access tokens representing the user and the selected MCP server.
  name: OAuth
  type: oauth2
slug: mintmcp-authentication
source_filename: mintmcp-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mintmcp.com/docs/authentication-models
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mintmcp.com/docs/authentication-models\nsources:\n- https://www.mintmcp.com/docs/authentication-models\n- https://www.mintmcp.com/docs/stdio-oauth-howto\n- https://www.mintmcp.com/docs/security/authentication-identity\n- https://www.mintmcp.com/docs/hosted-connector-oauth\ndescription: Client authentication\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Every MCP server exposes an OAuth 2.0 endpoint. AI clients use this to get access tokens representing the user and the selected MCP\n    server.\ndocs: https://www.mintmcp.com/docs/authentication-models\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mintmcp/refs/heads/main/authentication/mintmcp-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Platform
- Enterprise
- Security
- Integration
---
