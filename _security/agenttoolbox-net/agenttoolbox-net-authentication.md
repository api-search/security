---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agenttoolbox-net-directory-api-openapi.yml
  format: yaml
  label: Agent Toolbox Directory API
  slug: agenttoolbox-net-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenttoolbox-net/openapi/agenttoolbox-net-directory-api-openapi.yml
- filename: agenttoolbox-net-tools-api-openapi.yml
  format: yaml
  label: Agent Toolbox Tools API
  slug: agenttoolbox-net-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenttoolbox-net/openapi/agenttoolbox-net-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agenttoolbox Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Toolbox declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Toolbox
provider_slug: agenttoolbox-net
scheme_count: 1
schemes:
- evidence: The client sends an ordinary MCP request with no token, and the server answers with HTTP 401 and a WWW-Authenticate header.
  header: Authorization
  how_to_obtain: Clients register with the authorization server (via pre‑registered credentials, client ID metadata documents, or dynamic client registration) to obtain a client ID and then request audience‑bound tokens as described in the OAuth flow.
  location: header
  name: Bearer
  type: http-bearer
slug: agenttoolbox-net-authentication
source_filename: agenttoolbox-net-authentication.yml
source_heading: Authentication Profile
source_url: https://agenttoolbox.net/blog/oauth-for-remote-mcp-servers
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agenttoolbox.net/blog/oauth-for-remote-mcp-servers\nsources:\n- https://agenttoolbox.net/blog/oauth-for-remote-mcp-servers\n- https://agenttoolbox.net/tools/tokens\n- https://agenttoolbox.net/blog/budget-caps-for-agent-runs\n- https://agenttoolbox.net/blog/reasoning-models-in-agent-loops\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The client sends an ordinary MCP request with no token, and the server answers with HTTP 401 and a WWW-Authenticate header.\n  location: header\n  header: Authorization\n  how_to_obtain: Clients register with the authorization server (via pre‑registered credentials, client ID metadata documents, or dynamic client\n    registration) to obtain a client ID and then request audience‑bound tokens as described in the OAuth flow.\ndocs: https://agenttoolbox.net/blog/oauth-for-remote-mcp-servers\n"
source_yaml_url: https://artifacts.apis.io/agenttoolbox-net/authentication/agenttoolbox-net-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Tools
- Free
- Browser
- Agents
---
