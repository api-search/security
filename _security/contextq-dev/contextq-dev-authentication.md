---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contextq-dev-openapi-generated.yml
  format: yaml
  label: ContextQ API
  slug: contextq-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextq-dev/openapi/_ae-authored/contextq-dev-openapi-generated.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ContextQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContextQ declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ContextQ
provider_slug: contextq-dev
scheme_count: 1
schemes:
- evidence: Other agents Codex, Gemini CLI, Windsurf, and Cline all support MCP. Point them at the same streamable HTTP endpoint, https://app.contextq.dev/mcp , with your API key as a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Create an API key in the dashboard under Settings > API Keys.
  location: header
  name: API Key
  type: http-bearer
slug: contextq-dev-authentication
source_filename: contextq-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://contextq.dev/getting-started/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://contextq.dev/getting-started/\nsources:\n- https://contextq.dev/getting-started/\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Other agents Codex, Gemini CLI, Windsurf, and Cline all support MCP. Point them at the same streamable HTTP endpoint, https://app.contextq.dev/mcp\n    , with your API key as a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard under Settings > API Keys.\ndocs: https://contextq.dev/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/contextq-dev/authentication/contextq-dev-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Persistent
- Context
- Agents
- Platform
---
