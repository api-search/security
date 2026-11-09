---
anonymous_access: false
api_key_in: []
api_specs:
- filename: connic-co-public-openapi.json
  format: json
  label: connic API Public API
  slug: connic-api-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connic-co/openapi/_original/connic-co-public-openapi.json
auth_types: []
description: Authentication methods for Connic APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Connic Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connic declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Connic
provider_slug: connic-co
scheme_count: 2
schemes:
- evidence: 'Send the key as a bearer token:


    ```http

    Authorization: Bearer cnc_your_api_key

    ```'
  header: Authorization
  how_to_obtain: Create the key in Project Settings → API Keys & MCP Auth; the key is displayed only once.
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://mcp.connic.co/oauth/authorize
  evidence: Use the browser-based OAuth flow for connic MCP.
  header: Authorization
  how_to_obtain: Register a client via Dynamic Client Registration; then perform Authorization Code flow with PKCE S256 using a browser where a signed‑in user consents to the requested scopes.
  location: header
  name: connic MCP OAuth
  scopes:
  - mcp:read
  - mcp:write
  token_url: https://mcp.connic.co/oauth/token
  type: oauth2
slug: connic-co-authentication
source_filename: connic-co-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.connic.co/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.connic.co/.well-known/oauth-protected-resource/mcp\nsources:\n- https://mcp.connic.co/.well-known/oauth-protected-resource/mcp\n- https://mcp.connic.co/.well-known/oauth-authorization-server\n- https://connic.co/auth.md\n- https://connic.co/docs/v1/reference/rest-api\ndescription: Authentication methods for Connic APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key as a bearer token:\n\n\n    ```http\n\n    Authorization: Bearer cnc_your_api_key\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Create the key in Project Settings → API Keys & MCP Auth; the key is displayed only once.\n- type: oauth2\n  name: connic MCP OAuth\n  evidence: Use the browser-based OAuth flow for connic MCP.\n  location: header\n  header: Authorization\n  token_url: https://mcp.connic.co/oauth/token\n  authorize_url: https://mcp.connic.co/oauth/authorize\n\
  \  scopes:\n  - mcp:read\n  - mcp:write\n  how_to_obtain: Register a client via Dynamic Client Registration; then perform Authorization Code flow with PKCE S256 using a browser where\n    a signed‑in user consents to the requested scopes.\ndocs: https://mcp.connic.co/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/connic-co/authentication/connic-co-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Platform
- Munich
- Automation
---
