---
anonymous_access: false
api_key_in: []
api_specs:
- filename: freeappstore-online-openapi-generated.yml
  format: yaml
  label: FreeAppStore API
  slug: freeappstore-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeappstore-online/openapi/_ae-authored/freeappstore-online-openapi-generated.yml
auth_types: []
description: Authentication methods supported by the FreeAppStore MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FreeAppStore Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreeAppStore declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FreeAppStore
provider_slug: freeappstore-online
scheme_count: 2
schemes:
- evidence: 'The MCP server supports two auth methods: OAuth 2.1 (automatic via mcp-remote ) — recommended.'
  how_to_obtain: Automatic via mcp-remote which redirects to GitHub sign‑in and provisions a scoped access token.
  name: OAuth 2.1
  type: oauth2
- evidence: 'Bearer token — pass a FAS session token directly via Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Obtain a first‑party FAS session token (e.g., via CLI fas login or console sign‑in) and include it in the Authorization header.
  location: header
  name: Bearer token
  type: http-bearer
slug: freeappstore-online-authentication
source_filename: freeappstore-online-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.freeappstore.online/mcp/#authentication
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.freeappstore.online/mcp/#authentication\nsources:\n- https://docs.freeappstore.online/mcp/#authentication\ndescription: Authentication methods supported by the FreeAppStore MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'The MCP server supports two auth methods: OAuth 2.1 (automatic via mcp-remote ) — recommended.'\n  how_to_obtain: Automatic via mcp-remote which redirects to GitHub sign‑in and provisions a scoped access token.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bearer token — pass a FAS session token directly via Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a first‑party FAS session token (e.g., via CLI fas login or console sign‑in) and include it in the Authorization header.\ndocs: https://docs.freeappstore.online/mcp/#authentication\n"
source_yaml_url: https://artifacts.apis.io/freeappstore-online/authentication/freeappstore-online-authentication.yml
summary_line: 2 schemes
tags:
- Web App
- Free
- No Ads
- Productivity
- Finance
- Health and Fitness
- Learning
- Utilities
---
