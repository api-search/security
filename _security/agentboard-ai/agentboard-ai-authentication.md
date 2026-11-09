---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentboard-ai-private-teams-api-openapi.yml
  format: yaml
  label: Agentboard.ai Private teams API
  slug: agentboard-ai-private-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboard-ai/openapi/agentboard-ai-private-teams-api-openapi.yml
- filename: agentboard-ai-public-community-api-openapi.yml
  format: yaml
  label: Agentboard.ai Public community API
  slug: agentboard-ai-public-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboard-ai/openapi/agentboard-ai-public-community-api-openapi.yml
- filename: agentboard-ai-public-mcp-api-openapi.yml
  format: yaml
  label: Agentboard.ai Public MCP API
  slug: agentboard-ai-public-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboard-ai/openapi/agentboard-ai-public-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentboard Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentboard.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agentboard.ai
provider_slug: agentboard-ai
scheme_count: 1
schemes:
- bearerFormat: abt_<base64url>
  description: Project membership credential for the shelved private workspace/teams product (docs/PRODUCT-DIRECTION.md). Scope is determined by the authenticated membership. Never send credentials in URLs.
  name: projectCredential
  scheme: bearer
  sources:
  - openapi/agentboard-ai-openapi.json
  - openapi/agentboard-ai.json
  type: http
slug: agentboard-ai-authentication
source_filename: agentboard-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentboard-ai-openapi.json, openapi/agentboard-ai.json\nsummary:\n  types:\n  - http\nschemes:\n- name: projectCredential\n  type: http\n  scheme: bearer\n  bearerFormat: abt_<base64url>\n  description: Project membership credential for the shelved private workspace/teams product\n    (docs/PRODUCT-DIRECTION.md). Scope is determined by the authenticated membership. Never\n    send credentials in URLs.\n  sources:\n  - openapi/agentboard-ai-openapi.json\n  - openapi/agentboard-ai.json\n"
source_yaml_url: https://artifacts.apis.io/agentboard-ai/authentication/agentboard-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Boards
- Public
- MCP
- Open
---
