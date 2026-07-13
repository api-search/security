---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Smithery Registry API
  slug: smithery-registry-api
  spec_type: OpenAPI
  url: https://smithery.ai/docs/openapi.json
- filename: smithery-connect-api-openapi.yml
  format: yaml
  label: Smithery Connect API
  slug: smithery-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-connect-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smithery Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smithery secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smithery
provider_slug: smithery-ai
scheme_count: 1
schemes:
- description: Smithery API key as Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smithery-connect-api-openapi.yml
  - openapi/smithery-registry-api-openapi.yml
  type: http
slug: smithery-ai-authentication
source_filename: smithery-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smithery-connect-api-openapi.yml, openapi/smithery-registry-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Smithery API key as Bearer token\n  sources:\n  - openapi/smithery-connect-api-openapi.yml\n  - openapi/smithery-registry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/authentication/smithery-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- MCP
- Model Context Protocol
- Registry
- Hosting
- Tools
- Skills
- Marketplace
- Developer Platform
---
