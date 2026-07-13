---
api_key_in: []
api_specs:
- filename: smithery-openapi.json
  format: json
  label: Smithery Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smithery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smithery secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smithery
provider_slug: smithery
scheme_count: 1
schemes:
- description: Smithery API key as Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smithery-documented-openapi.yml
  - openapi/smithery-openapi.json
  type: http
slug: smithery-authentication
source_filename: smithery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smithery-documented-openapi.yml, openapi/smithery-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Smithery API key as Bearer token\n  sources:\n  - openapi/smithery-documented-openapi.yml\n  - openapi/smithery-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/authentication/smithery-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Large Language Models
- MCP
- Model Context Protocol
- AI Agents
- Developer Tools
- Registry
- Skills
- Tool Discovery
---
