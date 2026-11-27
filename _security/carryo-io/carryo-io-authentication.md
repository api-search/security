---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carryo-io-health-api-openapi.yml
  format: yaml
  label: Carryo Health API
  slug: carryo-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-health-api-openapi.yml
- filename: carryo-io-mcp-api-openapi.yml
  format: yaml
  label: Carryo MCP API
  slug: carryo-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-mcp-api-openapi.yml
- filename: carryo-io-well-known-api-openapi.yml
  format: yaml
  label: Carryo .well Known API
  slug: carryo-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-well-known-api-openapi.yml
auth_types: []
description: Carryo MCP uses OAuth 2.0 bearer token authentication sent in the HTTP Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Carryo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carryo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Carryo
provider_slug: carryo-io
scheme_count: 1
schemes:
- evidence: '"bearer_methods_supported":["header"]'
  header: Authorization
  location: header
  name: Bearer
  scopes:
  - artifact.read
  - artifact.write
  - artifact.revoke
  type: http-bearer
slug: carryo-io-authentication
source_filename: carryo-io-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.carryo.io/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.carryo.io/.well-known/oauth-protected-resource/mcp\nsources:\n- https://mcp.carryo.io/.well-known/oauth-protected-resource/mcp\n- https://carryo.io/get-started\n- https://carryo.io/docs\ndescription: Carryo MCP uses OAuth 2.0 bearer token authentication sent in the HTTP Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '\"bearer_methods_supported\":[\"header\"]'\n  location: header\n  header: Authorization\n  scopes:\n  - artifact.read\n  - artifact.write\n  - artifact.revoke\ndocs: https://mcp.carryo.io/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/carryo-io/authentication/carryo-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Website Publishing
- Content Generation
- Software-as-a-Service
- Low-Code
---
