---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allmcps-a2a-api-openapi.yml
  format: yaml
  label: AllMCPs A2a API
  slug: allmcps-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-a2a-api-openapi.yml
- filename: allmcps-acp-api-openapi.yml
  format: yaml
  label: AllMCPs Acp API
  slug: allmcps-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-acp-api-openapi.yml
- filename: allmcps-ads-api-openapi.yml
  format: yaml
  label: AllMCPs Ads API
  slug: allmcps-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-ads-api-openapi.yml
- filename: allmcps-agent-api-openapi.yml
  format: yaml
  label: AllMCPs Agent API
  slug: allmcps-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-agent-api-openapi.yml
- filename: allmcps-badge-api-openapi.yml
  format: yaml
  label: AllMCPs Badge API
  slug: allmcps-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-badge-api-openapi.yml
- filename: allmcps-boost-api-openapi.yml
  format: yaml
  label: AllMCPs Boost API
  slug: allmcps-boost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-boost-api-openapi.yml
- filename: allmcps-categories-api-openapi.yml
  format: yaml
  label: AllMCPs Categories API
  slug: allmcps-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-categories-api-openapi.yml
- filename: allmcps-health-api-openapi.yml
  format: yaml
  label: AllMCPs Health API
  slug: allmcps-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-health-api-openapi.yml
- filename: allmcps-mcp-api-openapi.yml
  format: yaml
  label: AllMCPs MCP API
  slug: allmcps-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-mcp-api-openapi.yml
- filename: allmcps-search-api-openapi.yml
  format: yaml
  label: AllMCPs Search API
  slug: allmcps-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-search-api-openapi.yml
- filename: allmcps-servers-api-openapi.yml
  format: yaml
  label: AllMCPs Servers API
  slug: allmcps-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-servers-api-openapi.yml
- filename: allmcps-submit-api-openapi.yml
  format: yaml
  label: AllMCPs Submit API
  slug: allmcps-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-submit-api-openapi.yml
auth_types: []
description: Authentication methods for remote MCP servers as described in AllMCPs documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AllMCPs Authentication
name_suffix: Authentication
oauth_flows: []
overview: AllMCPs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AllMCPs
provider_slug: allmcps
scheme_count: 1
schemes:
- evidence: 'For standard server-to-server or pre-authenticated agent sessions, clients pass an HTTP Authorization header containing a JSON Web Token (JWT) or scoped API key during transport connection:'
  header: Authorization
  location: header
  name: JWT Bearer Token
  type: http-bearer
slug: allmcps-authentication
source_filename: allmcps-authentication.yml
source_heading: Authentication Profile
source_url: https://allmcps.com/blog/mcp-oauth-authorization-flow
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://allmcps.com/blog/mcp-oauth-authorization-flow\nsources:\n- https://allmcps.com/blog/mcp-oauth-authorization-flow\n- https://allmcps.com/blog/how-mcp-sampling-works-guide\n- https://allmcps.com/blog/securing-remote-mcp-servers-authentication-guide\ndescription: Authentication methods for remote MCP servers as described in AllMCPs documentation.\nschemes:\n- type: http-bearer\n  name: JWT Bearer Token\n  evidence: 'For standard server-to-server or pre-authenticated agent sessions, clients pass an HTTP Authorization header containing a JSON Web\n    Token (JWT) or scoped API key during transport connection:'\n  location: header\n  header: Authorization\ndocs: https://allmcps.com/blog/mcp-oauth-authorization-flow\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/allmcps/authentication/allmcps-authentication.yml
summary_line: 1 scheme
tags:
- Directory
- MCP
- AI Agents
- Developer Tools
- Search & Data Extraction
- Finance & Fintech
- Communications
- Knowledge & Memory
---
