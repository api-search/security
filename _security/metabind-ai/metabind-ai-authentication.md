---
anonymous_access: false
api_key_in: []
api_specs:
- filename: metabind-ai-bindjs-openapi.json
  format: json
  label: OpenAPI Plant Store Bindjs API
  slug: openapi-plant-store-bindjs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/metabind-ai/openapi/_original/metabind-ai-bindjs-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Metabind Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: metabind-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: metabind-ai
provider_slug: metabind-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT bearer token for admin (/app/v1/) routes
  scheme: bearer
  type: http
- description: API key for client (/api/v1/) routes, optionally scoped
  in: header
  name: x-api-key
  type: apiKey
slug: metabind-ai-authentication
source_filename: metabind-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: \"https://docs.metabind.ai/rest/authentication.md\"\nschemes:\n  - type: \"http\"\n    scheme: \"bearer\"\n    bearerFormat: \"JWT\"\n    description: \"JWT bearer token for admin (/app/v1/) routes\"\n  - type: \"apiKey\"\n    name: \"x-api-key\"\n    in: \"header\"\n    description: \"API key for client (/api/v1/) routes, optionally scoped\"\n"
source_yaml_url: https://artifacts.apis.io/metabind-ai/authentication/metabind-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- MCP
- Agents
- Platform
- Integration
---
