---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foundry-mcp-com-public-api-openapi.yml
  format: yaml
  label: foundry-mcp-com Public API
  slug: foundry-mcp-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundry-mcp-com/openapi/foundry-mcp-com-public-api-openapi.yml
- filename: foundry-mcp-com-tier-adventurer-api-openapi.yml
  format: yaml
  label: foundry-mcp-com Tier Adventurer API
  slug: foundry-mcp-com-tier-adventurer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundry-mcp-com/openapi/foundry-mcp-com-tier-adventurer-api-openapi.yml
- filename: foundry-mcp-com-tier-dm-api-openapi.yml
  format: yaml
  label: foundry-mcp-com Tier Dm API
  slug: foundry-mcp-com-tier-dm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundry-mcp-com/openapi/foundry-mcp-com-tier-dm-api-openapi.yml
- filename: foundry-mcp-com-tier-free-api-openapi.yml
  format: yaml
  label: foundry-mcp-com Tier Free API
  slug: foundry-mcp-com-tier-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundry-mcp-com/openapi/foundry-mcp-com-tier-free-api-openapi.yml
- filename: foundry-mcp-com-tier-guest-api-openapi.yml
  format: yaml
  label: foundry-mcp-com Tier Guest API
  slug: foundry-mcp-com-tier-guest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundry-mcp-com/openapi/foundry-mcp-com-tier-guest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Foundry Mcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: foundry-mcp-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: foundry-mcp-com
provider_slug: foundry-mcp-com
scheme_count: 1
schemes:
- description: 'API key issued via foundry-mcp Patreon registration. Include as `Authorization: Bearer <key>` on every authenticated endpoint.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/foundry-mcp-com-openapi.json
  type: http
slug: foundry-mcp-com-authentication
source_filename: foundry-mcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/foundry-mcp-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued via foundry-mcp Patreon registration. Include as `Authorization:\n    Bearer <key>` on every authenticated endpoint.'\n  sources:\n  - openapi/foundry-mcp-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/foundry-mcp-com/authentication/foundry-mcp-com-authentication.yml
summary_line: http · 1 scheme
tags:
- FoundryVTT
- MCP
- AI
- Gaming
- Automation
---
