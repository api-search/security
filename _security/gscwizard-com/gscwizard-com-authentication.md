---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gscwizard-com-api-openapi.json
  format: json
  label: GSC Wizard REST API API
  slug: gsc-wizard-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gscwizard-com/openapi/_original/gscwizard-com-api-openapi.json
auth_types: []
description: Authentication methods for GSC Wizard MCP and REST API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GSC Wizard Authentication
name_suffix: Authentication
oauth_flows: []
overview: GSC Wizard declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GSC Wizard
provider_slug: gscwizard-com
scheme_count: 2
schemes:
- authorize_url: https://tool.gscwizard.com/oauth/authorize
  evidence: OAuth 2.1 (authorization code + PKCE) | An MCP client or agent acting for a user who can sign in interactively
  header: Authorization
  how_to_obtain: Register a client dynamically by POSTing client metadata to https://tool.gscwizard.com/api/oauth/register, then follow the authorization‑code with PKCE flow (send user to the authorize URL, exchange code at the token URL).
  location: header
  name: OAuth 2.1 (authorization code + PKCE)
  scopes:
  - mcp:read
  - mcp:write
  token_url: https://tool.gscwizard.com/api/oauth/token
  type: oauth2
- evidence: API key | Scripts, servers, CI, and MCP clients that cannot run OAuth
  header: Authorization
  how_to_obtain: User creates a key in the app under Account → API keys (https://tool.gscwizard.com/account/api-keys) and chooses a read or write scope. The key is shown once and used as a Bearer token.
  location: header
  name: API key
  type: apiKey
slug: gscwizard-com-authentication
source_filename: gscwizard-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.gscwizard.com/docs/bing.html
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.gscwizard.com/docs/bing.html\nsources:\n- https://www.gscwizard.com/docs/bing.html\n- https://www.gscwizard.com/auth.md\n- https://www.gscwizard.com/docs/mcp-and-chatgpt.html\ndescription: Authentication methods for GSC Wizard MCP and REST API\nschemes:\n- type: oauth2\n  name: OAuth 2.1 (authorization code + PKCE)\n  evidence: OAuth 2.1 (authorization code + PKCE) | An MCP client or agent acting for a user who can sign in interactively\n  location: header\n  header: Authorization\n  token_url: https://tool.gscwizard.com/api/oauth/token\n  authorize_url: https://tool.gscwizard.com/oauth/authorize\n  scopes:\n  - mcp:read\n  - mcp:write\n  how_to_obtain: Register a client dynamically by POSTing client metadata to https://tool.gscwizard.com/api/oauth/register, then follow the authorization‑code\n    with PKCE flow (send user to the authorize URL, exchange code at the token\
  \ URL).\n- type: apiKey\n  name: API key\n  evidence: API key | Scripts, servers, CI, and MCP clients that cannot run OAuth\n  location: header\n  header: Authorization\n  how_to_obtain: User creates a key in the app under Account → API keys (https://tool.gscwizard.com/account/api-keys) and chooses a read or write\n    scope. The key is shown once and used as a Bearer token.\ndocs: https://www.gscwizard.com/docs/bing.html\n"
source_yaml_url: https://artifacts.apis.io/gscwizard-com/authentication/gscwizard-com-authentication.yml
summary_line: 2 schemes
tags:
- SEO
- Analytics
- Data
- Growth
- Marketing
---
