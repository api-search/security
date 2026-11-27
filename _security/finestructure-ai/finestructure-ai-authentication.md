---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finestructure-ai-bridge-api-openapi.yml
  format: yaml
  label: Fine Structure Bridge API
  slug: finestructure-ai-bridge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-bridge-api-openapi.yml
- filename: finestructure-ai-discovery-api-openapi.yml
  format: yaml
  label: Fine Structure Discovery API
  slug: finestructure-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-discovery-api-openapi.yml
- filename: finestructure-ai-mcp-api-openapi.yml
  format: yaml
  label: Fine Structure MCP API
  slug: finestructure-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-mcp-api-openapi.yml
- filename: finestructure-ai-tools-api-openapi.yml
  format: yaml
  label: Fine Structure Tools API
  slug: finestructure-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-tools-api-openapi.yml
auth_types: []
description: Clients authenticate using a self‑serve API token sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fine Structure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fine Structure declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fine Structure
provider_slug: finestructure-ai
scheme_count: 1
schemes:
- evidence: Connect over MCP at https://finestructure.ai/api/mcp (Streamable HTTP, Bearer token), or over REST using the OpenAPI spec at https://finestructure.ai/openapi.json.
  header: Authorization
  how_to_obtain: Create a scoped API token at https://finestructure.ai/api-keys.
  location: header
  name: Bearer
  type: http-bearer
slug: finestructure-ai-authentication
source_filename: finestructure-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://finestructure.ai/docs/quickstart.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finestructure.ai/docs/quickstart.md\nsources:\n- https://finestructure.ai/docs/quickstart.md\ndescription: Clients authenticate using a self‑serve API token sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Connect over MCP at https://finestructure.ai/api/mcp (Streamable HTTP, Bearer token), or over REST using the OpenAPI spec at https://finestructure.ai/openapi.json.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a scoped API token at https://finestructure.ai/api-keys.\ndocs: https://finestructure.ai/docs/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/finestructure-ai/authentication/finestructure-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Automation
- Platform
- Integration
- Business
---
