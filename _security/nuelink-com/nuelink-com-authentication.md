---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuelink-com-openapi-generated.yml
  format: yaml
  label: Nuelink API
  slug: nuelink-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuelink-com/openapi/_ae-authored/nuelink-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Nuelink REST API and MCP server
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Nuelink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuelink declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Nuelink
provider_slug: nuelink-com
scheme_count: 3
schemes:
- evidence: 'The REST API uses API keys as bearer tokens. One header, every request: Authorization : Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Generate a key in Settings → API and copy it.
  location: header
  name: REST API Key
  type: http-bearer
- evidence: For compatibility with older clients, the API also accepts the key as an api_key query parameter.
  how_to_obtain: Generate a key in Settings → API and copy it.
  location: query
  name: REST API Key (query parameter – deprecated)
  type: apiKey
- authorize_url: https://mcp.nuelink.com/authorize
  evidence: 'Nuelink’s MCP server supports the full OAuth 2.1 flow: discovery, dynamic client registration, S256 PKCE, consent, code exchange, access tokens, refresh, and revocation.'
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Register a client via the dynamic registration endpoint (https://mcp.nuelink.com/register) and follow the OAuth 2.1 authorization flow.
  location: header
  name: MCP OAuth
  type: oauth2
slug: nuelink-com-authentication
source_filename: nuelink-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nuelink.com/guides/authentication/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nuelink.com/guides/authentication/\nsources:\n- https://docs.nuelink.com/guides/authentication/\n- https://docs.nuelink.com/mcp/authentication/\ndescription: Authentication methods for Nuelink REST API and MCP server\nschemes:\n- type: http-bearer\n  name: REST API Key\n  evidence: 'The REST API uses API keys as bearer tokens. One header, every request: Authorization : Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key in Settings → API and copy it.\n- type: apiKey\n  name: REST API Key (query parameter – deprecated)\n  evidence: For compatibility with older clients, the API also accepts the key as an api_key query parameter.\n  location: query\n  how_to_obtain: Generate a key in Settings → API and copy it.\n- type: oauth2\n  name: MCP OAuth\n  evidence: 'Nuelink’s MCP server supports the full OAuth 2.1 flow: discovery,\
  \ dynamic client registration, S256 PKCE, consent, code exchange,\n    access tokens, refresh, and revocation.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://mcp.nuelink.com/authorize\n  how_to_obtain: Register a client via the dynamic registration endpoint (https://mcp.nuelink.com/register) and follow the OAuth 2.1 authorization\n    flow.\ndocs: https://docs.nuelink.com/guides/authentication/\n"
source_yaml_url: https://artifacts.apis.io/nuelink-com/authentication/nuelink-com-authentication.yml
summary_line: 3 schemes
tags:
- Social Media Scheduling
- Automation
- AI Integration
- E-Commerce
- Agency Tools
- Content Management
---
