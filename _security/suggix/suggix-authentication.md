---
anonymous_access: false
api_key_in: []
api_specs:
- filename: suggix-indicators-api-openapi.yml
  format: yaml
  label: Suggix Indicators API
  slug: suggix-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-indicators-api-openapi.yml
- filename: suggix-industries-api-openapi.yml
  format: yaml
  label: Suggix Industries API
  slug: suggix-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-industries-api-openapi.yml
- filename: suggix-regions-api-openapi.yml
  format: yaml
  label: Suggix Regions API
  slug: suggix-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-regions-api-openapi.yml
- filename: suggix-search-api-openapi.yml
  format: yaml
  label: Suggix Search API
  slug: suggix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-search-api-openapi.yml
- filename: suggix-sources-api-openapi.yml
  format: yaml
  label: Suggix Sources API
  slug: suggix-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-sources-api-openapi.yml
- filename: suggix-statistics-api-openapi.yml
  format: yaml
  label: Suggix Statistics API
  slug: suggix-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/openapi/suggix-statistics-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Suggix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suggix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Suggix
provider_slug: suggix
scheme_count: 1
schemes:
- evidence: 'Set the MCP API key in your shell environment: export SUGGIX_MCP_API_KEY = "sgx_mcp_your_key"'
  header: Authorization
  how_to_obtain: Create or revoke a workspace MCP API key in Developer Settings and set it as the environment variable SUGGIX_MCP_API_KEY.
  location: header
  name: MCP API Key
  type: http-bearer
slug: suggix-authentication
source_filename: suggix-authentication.yml
source_heading: Authentication Profile
source_url: https://help.suggix.com/mcp/claude-code
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.suggix.com/mcp/claude-code\nsources:\n- https://help.suggix.com/mcp/claude-code\n- https://help.suggix.com/mcp/codex\n- https://help.suggix.com/mcp/cursor\nschemes:\n- type: http-bearer\n  name: MCP API Key\n  evidence: 'Set the MCP API key in your shell environment: export SUGGIX_MCP_API_KEY = \"sgx_mcp_your_key\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or revoke a workspace MCP API key in Developer Settings and set it as the environment variable SUGGIX_MCP_API_KEY.\ndocs: https://help.suggix.com/mcp/claude-code\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suggix/refs/heads/main/authentication/suggix-authentication.yml
summary_line: 1 scheme
tags:
- Software-as-a-Service
- Feedback
- Roadmaps
- Changelog
- Product Management
---
