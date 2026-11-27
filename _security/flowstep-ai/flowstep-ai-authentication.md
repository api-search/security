---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flowstep-ai-openapi-generated.yml
  format: yaml
  label: Flowstep API
  slug: flowstep-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowstep-ai/openapi/_ae-authored/flowstep-ai-openapi-generated.yml
auth_types: []
description: Authentication for Flowstep MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Flowstep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowstep declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Flowstep
provider_slug: flowstep-ai
scheme_count: 2
schemes:
- authorize_url: https://api.flowstep.ai/oauth/authorize
  evidence: The `/mcp` endpoint requires a Bearer token in the `Authorization` header.
  header: Authorization
  how_to_obtain: Clients obtain a token automatically through the OAuth 2.1 PKCE flow; a token can also be extracted manually from a logged‑in browser session for testing.
  location: header
  name: Bearer token
  type: http-bearer
- authorize_url: https://api.flowstep.ai/oauth/authorize
  evidence: MCP clients obtain one automatically through the OAuth 2.1 PKCE flow — there's no API key to create, paste, or rotate.
  flows:
  - authorization_code
  how_to_obtain: Clients open a browser window, log in with Flowstep credentials (email/password or Google), approve the consent screen, and the token is exchanged behind the scenes. No client ID needs to be pre‑registered.
  name: OAuth 2.1 PKCE flow
  type: oauth2
slug: flowstep-ai-authentication
source_filename: flowstep-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.flowstep.ai/mcp/authentication.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.flowstep.ai/mcp/authentication.md\nsources:\n- https://docs.flowstep.ai/mcp/authentication.md\n- https://docs.flowstep.ai/getting-started.md\n- https://docs.flowstep.ai/mcp/quickstart.md\ndescription: Authentication for Flowstep MCP\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: The `/mcp` endpoint requires a Bearer token in the `Authorization` header.\n  location: header\n  header: Authorization\n  authorize_url: https://api.flowstep.ai/oauth/authorize\n  how_to_obtain: Clients obtain a token automatically through the OAuth 2.1 PKCE flow; a token can also be extracted manually from a logged‑in\n    browser session for testing.\n- type: oauth2\n  name: OAuth 2.1 PKCE flow\n  evidence: MCP clients obtain one automatically through the OAuth 2.1 PKCE flow — there's no API key to create, paste, or rotate.\n  flows:\n  - authorization_code\n  authorize_url:\
  \ https://api.flowstep.ai/oauth/authorize\n  how_to_obtain: Clients open a browser window, log in with Flowstep credentials (email/password or Google), approve the consent screen, and the\n    token is exchanged behind the scenes. No client ID needs to be pre‑registered.\ndocs: https://docs.flowstep.ai/mcp/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/flowstep-ai/authentication/flowstep-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Design
- UI
- Collaboration
- Software-as-a-Service
---
