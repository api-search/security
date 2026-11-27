---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contio-ai-openapi-generated.yml
  format: yaml
  label: Contio API
  slug: contio-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contio-ai/openapi/_ae-authored/contio-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Contio hosted MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Contio
provider_slug: contio-ai
scheme_count: 2
schemes:
- authorize_url: https://app.contio.ai/v1/oauth/authorize
  evidence: 'Start authorization at https://app.contio.ai/v1/oauth/authorize with PKCE ( S256 ) and the scopes you need. Exchange the code at https://api.contio.ai/v1/oauth/token . The client sends the resulting cto_at_v1_... token on every MCP request: Authorization: Bearer cto_at_v1_...'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register the client (first‑party client_id) or use Dynamic Client Registration, then follow the PKCE authorization code flow to obtain an access token.
  location: header
  name: OAuth 2.1 + PKCE
  type: http-bearer
- evidence: PATs cannot carry the workspace:read / workspace:write scopes; for workspace‑admin tooling, use a workspace API key ( cto_wk_v1_ ) as the bearer token instead.
  header: Authorization
  how_to_obtain: Generate a workspace API key in the Contio app (details not provided on the page).
  location: header
  name: Workspace API Key
  type: http-bearer
slug: contio-ai-authentication
source_filename: contio-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.contio.ai/user-api/guides/hosted-mcp/#connect-your-mcp-client
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.contio.ai/user-api/guides/hosted-mcp/#connect-your-mcp-client\nsources:\n- https://docs.contio.ai/user-api/guides/hosted-mcp/#connect-your-mcp-client\n- https://helpcenter.contio.ai/en/\ndescription: Authentication methods for Contio hosted MCP server\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 + PKCE\n  evidence: 'Start authorization at https://app.contio.ai/v1/oauth/authorize with PKCE ( S256 ) and the scopes you need. Exchange the code at\n    https://api.contio.ai/v1/oauth/token . The client sends the resulting cto_at_v1_... token on every MCP request: Authorization: Bearer cto_at_v1_...'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://app.contio.ai/v1/oauth/authorize\n  how_to_obtain: Register the client (first‑party client_id) or use Dynamic Client Registration, then follow the PKCE authorization code\
  \ flow\n    to obtain an access token.\n- type: http-bearer\n  name: Workspace API Key\n  evidence: PATs cannot carry the workspace:read / workspace:write scopes; for workspace‑admin tooling, use a workspace API key ( cto_wk_v1_ )\n    as the bearer token instead.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a workspace API key in the Contio app (details not provided on the page).\ndocs: https://docs.contio.ai/user-api/guides/hosted-mcp/#connect-your-mcp-client\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/contio-ai/authentication/contio-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Productivity
- Meetings
- Software-as-a-Service
- Collaboration
---
