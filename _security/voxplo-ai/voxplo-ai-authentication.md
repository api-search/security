---
anonymous_access: false
api_key_in: []
api_specs:
- filename: voxplo-ai-agent-api-openapi.yml
  format: yaml
  label: Voxplo Agent API
  slug: voxplo-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/voxplo-ai/openapi/voxplo-ai-agent-api-openapi.yml
auth_types: []
description: Authentication methods for Voxplo
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Voxplo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voxplo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Voxplo
provider_slug: voxplo-ai
scheme_count: 2
schemes:
- authorize_url: https://mcp.voxplo.ai/authorize
  evidence: Begin the authorization-code flow (with PKCE) at https://mcp.voxplo.ai/authorize. A human approves by pasting a Voxplo Agent API key (bys_ak_...) from the dashboard at https://voxplo.ai/account.
  flows:
  - authorization_code
  how_to_obtain: Register a client via POST https://mcp.voxplo.ai/register to obtain a client_id, then perform the OAuth2 authorization‑code flow with PKCE.
  name: Voxplo MCP OAuth2
  scopes:
  - voxplo.calls.read
  - voxplo.calls.place
  type: oauth2
- evidence: 'curl -X POST https://api.voxplo.ai/v1/agent/calls \ -H "Authorization: Bearer bys_ak_YOUR_KEY" \ -H "Content-Type: application/json"'
  header: Authorization
  how_to_obtain: Create an agent key in the Voxplo dashboard under Account → Developers; the key starts with bys_ak_ and is shown only once.
  location: header
  name: Agent API key
  type: http-bearer
slug: voxplo-ai-authentication
source_filename: voxplo-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.voxplo.ai/auth.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.voxplo.ai/auth.md\nsources:\n- https://mcp.voxplo.ai/auth.md\n- https://www.voxplo.ai/docs/agent-api/quickstart\n- https://www.voxplo.ai/docs/account\ndescription: Authentication methods for Voxplo\nschemes:\n- type: oauth2\n  name: Voxplo MCP OAuth2\n  evidence: Begin the authorization-code flow (with PKCE) at https://mcp.voxplo.ai/authorize. A human approves by pasting a Voxplo Agent API key\n    (bys_ak_...) from the dashboard at https://voxplo.ai/account.\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.voxplo.ai/authorize\n  scopes:\n  - voxplo.calls.read\n  - voxplo.calls.place\n  how_to_obtain: Register a client via POST https://mcp.voxplo.ai/register to obtain a client_id, then perform the OAuth2 authorization‑code flow\n    with PKCE.\n- type: http-bearer\n  name: Agent API key\n  evidence: 'curl -X POST https://api.voxplo.ai/v1/agent/calls \\\
  \ -H \"Authorization: Bearer bys_ak_YOUR_KEY\" \\ -H \"Content-Type: application/json\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an agent key in the Voxplo dashboard under Account → Developers; the key starts with bys_ak_ and is shown only once.\ndocs: https://mcp.voxplo.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/voxplo-ai/authentication/voxplo-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Voice
- MCP
---
