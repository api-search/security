---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elevenflo-com-openapi-generated.yml
  format: yaml
  label: ElevenFlo API
  slug: elevenflo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elevenflo-com/openapi/_ae-authored/elevenflo-com-openapi-generated.yml
auth_types: []
description: ElevenFlo MCP uses OAuth 2.1 authorization code flow with PKCE for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ElevenFlo Authentication
name_suffix: Authentication
oauth_flows: []
overview: ElevenFlo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ElevenFlo
provider_slug: elevenflo-com
scheme_count: 1
schemes:
- evidence: Interactive access uses remote MCP over HTTP (Streamable HTTP transport). You sign in with your ElevenFlo web-app account, and every authorization request uses the OAuth 2.1 authorization code flow with PKCE.
  flows:
  - authorization_code
  how_to_obtain: Create an OAuth client in the ElevenFlo web app (or use a pre‑registered client). The client will receive a client ID (and optionally a client secret) which is used in the authorization code with PKCE flow.
  name: ElevenFlo MCP OAuth
  scopes:
  - mcp:access
  type: oauth2
slug: elevenflo-com-authentication
source_filename: elevenflo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://elevenflo.com/docs/mcp/setup
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://elevenflo.com/docs/mcp/setup\nsources:\n- https://elevenflo.com/docs/mcp/setup\n- https://elevenflo.com/docs/mcp/permissions-and-data-access\ndescription: ElevenFlo MCP uses OAuth 2.1 authorization code flow with PKCE for authentication.\nschemes:\n- type: oauth2\n  name: ElevenFlo MCP OAuth\n  evidence: Interactive access uses remote MCP over HTTP (Streamable HTTP transport). You sign in with your ElevenFlo web-app account, and every\n    authorization request uses the OAuth 2.1 authorization code flow with PKCE.\n  flows:\n  - authorization_code\n  scopes:\n  - mcp:access\n  how_to_obtain: Create an OAuth client in the ElevenFlo web app (or use a pre‑registered client). The client will receive a client ID (and optionally\n    a client secret) which is used in the authorization code with PKCE flow.\ndocs: https://elevenflo.com/docs/mcp/setup\n"
source_yaml_url: https://artifacts.apis.io/elevenflo-com/authentication/elevenflo-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Data
- Research
- Bankruptcy
---
