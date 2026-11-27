---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gessa-ai-openapi-generated.yml
  format: yaml
  label: Gessa API
  slug: gessa-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gessa-ai/openapi/_ae-authored/gessa-ai-openapi-generated.yml
auth_types: []
description: OAuth 2.1 authorization‑code flow with PKCE S256
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gessa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gessa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gessa
provider_slug: gessa-ai
scheme_count: 1
schemes:
- authorize_url: https://api.gessa.ai/.well-known/oauth-authorization-server (authorization_endpoint value)
  evidence: Gessa exposes an authenticated MCP service at `https://api.gessa.ai/mcp/rpc`. This document tells an agent how to discover and complete the OAuth 2.1 authorization-code flow with PKCE S256.
  flows:
  - authorization_code
  how_to_obtain: Dynamic client registration via POST to the registration_endpoint as described in the Register section.
  name: OAuth 2.1
  scopes:
  - mcp:read
  - mcp:write
  - mcp:admin
  - mcp:platform
  type: oauth2
slug: gessa-ai-authentication
source_filename: gessa-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://gessa.ai/auth.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gessa.ai/auth.md\nsources:\n- https://gessa.ai/auth.md\n- https://gessa.ai/developers/\n- https://gessa.ai/docs/creator/mcp/quickstart/\n- https://gessa.ai/docs/start/quickstart/\ndescription: OAuth 2.1 authorization‑code flow with PKCE S256\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Gessa exposes an authenticated MCP service at `https://api.gessa.ai/mcp/rpc`. This document tells an agent how to discover and complete\n    the OAuth 2.1 authorization-code flow with PKCE S256.\n  flows:\n  - authorization_code\n  authorize_url: https://api.gessa.ai/.well-known/oauth-authorization-server (authorization_endpoint value)\n  scopes:\n  - mcp:read\n  - mcp:write\n  - mcp:admin\n  - mcp:platform\n  how_to_obtain: Dynamic client registration via POST to the registration_endpoint as described in the Register section.\ndocs: https://gessa.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/gessa-ai/authentication/gessa-ai-authentication.yml
summary_line: 1 scheme
tags:
- Gaming
- Artificial Intelligence
- Browser
- Multiplayer
- Platform
---
