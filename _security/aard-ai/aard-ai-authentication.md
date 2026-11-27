---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aard-ai-status-api-openapi.yml
  format: yaml
  label: Aard Status API
  slug: aard-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aard-ai/openapi/aard-ai-status-api-openapi.yml
- filename: aard-ai-tools-api-openapi.yml
  format: yaml
  label: Aard Tools API
  slug: aard-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aard-ai/openapi/aard-ai-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aard
provider_slug: aard-ai
scheme_count: 1
schemes:
- bearerFormat: aard_live_<key>
  description: An Aard API key from https://aard.ai/account/keys. Shown once on creation; revocable there.
  scheme: bearer
  type: http
slug: aard-ai-authentication
source_filename: aard-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://aard.ai/docs/mcp-oauth\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: aard_live_<key>\n    description: An Aard API key from https://aard.ai/account/keys. Shown once on creation; revocable there.\n"
source_yaml_url: https://artifacts.apis.io/aard-ai/authentication/aard-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Data
- Macroeconomics
- MCP
---
