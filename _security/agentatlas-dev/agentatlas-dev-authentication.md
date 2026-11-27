---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentatlas-dev-openapi-generated.yml
  format: yaml
  label: AgentAtlas API
  slug: agentatlas-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentatlas-dev/openapi/_ae-authored/agentatlas-dev-openapi-generated.yml
auth_types: []
description: Authentication schemes documented for AgentAtlas providers.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: AgentAtlas Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentAtlas declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AgentAtlas
provider_slug: agentatlas-dev
scheme_count: 3
schemes:
- evidence: API keys go in environment variables, a .env file, command line switches or the YAML config.
  location: environment variable
  name: API key
  type: apiKey
- evidence: '"headers": { "Authorization": "Bearer ${API_TOKEN}" }"'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: For others, add an oauth object.
  name: OAuth
  scopes:
  - read
  - write
  type: oauth2
slug: agentatlas-dev-authentication
source_filename: agentatlas-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://agentatlas.dev/guides/aider-conventions
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentatlas.dev/guides/aider-conventions\nsources:\n- https://agentatlas.dev/guides/aider-conventions\n- https://agentatlas.dev/guides/kiro-mcp-json\n- https://agentatlas.dev/mcp/category/auth\n- https://agentatlas.dev/mcp/clerk\ndescription: Authentication schemes documented for AgentAtlas providers.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: API keys go in environment variables, a .env file, command line switches or the YAML config.\n  location: environment variable\n- type: http-bearer\n  name: Bearer token\n  evidence: '\"headers\": { \"Authorization\": \"Bearer ${API_TOKEN}\" }\"'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth\n  evidence: For others, add an oauth object.\n  scopes:\n  - read\n  - write\ndocs: https://agentatlas.dev/guides/aider-conventions\n"
source_yaml_url: https://artifacts.apis.io/agentatlas-dev/authentication/agentatlas-dev-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Agents
- MCP
- Tools
- Platform
---
