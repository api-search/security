---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpemails-com-openapi-generated.yml
  format: yaml
  label: MCP Emails API
  slug: mcpemails-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpemails-com/openapi/_ae-authored/mcpemails-com-openapi-generated.yml
auth_types: []
description: Authentication methods for MCP Emails API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MCP Emails Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCP Emails declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MCP Emails
provider_slug: mcpemails-com
scheme_count: 1
schemes:
- authorize_url: https://mcpemails.com/api/mcp
  evidence: OAuth 2.1, authorization code with PKCE. No API key.
  flows:
  - authorization_code
  how_to_obtain: Client runs the standard MCP OAuth flow, registers dynamically (RFC 7591) and authorizes with an authorization code plus PKCE; the token is listed in the Dashboard under API Keys as OAuth:<client name>.
  name: OAuth 2.1 Authorization Code with PKCE
  type: http-bearer
slug: mcpemails-com-authentication
source_filename: mcpemails-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcpemails.com/blog/oauth-vs-api-keys-ai-email-access
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcpemails.com/blog/oauth-vs-api-keys-ai-email-access\nsources:\n- https://mcpemails.com/blog/oauth-vs-api-keys-ai-email-access\n- https://mcpemails.com/docs/claude\n- https://mcpemails.com/docs/chatgpt\n- https://mcpemails.com/docs/cowork\ndescription: Authentication methods for MCP Emails API\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: OAuth 2.1, authorization code with PKCE. No API key.\n  flows:\n  - authorization_code\n  authorize_url: https://mcpemails.com/api/mcp\n  how_to_obtain: Client runs the standard MCP OAuth flow, registers dynamically (RFC 7591) and authorizes with an authorization code plus PKCE;\n    the token is listed in the Dashboard under API Keys as OAuth:<client name>.\ndocs: https://mcpemails.com/blog/oauth-vs-api-keys-ai-email-access\nnote: 1 extracted row(s) were dropped because their quote was not\
  \ on the page.\n"
source_yaml_url: https://artifacts.apis.io/mcpemails-com/authentication/mcpemails-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- MCP
- Cloud
- Services
---
