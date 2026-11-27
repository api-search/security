---
anonymous_access: false
api_key_in: []
api_specs:
- filename: charmnomicon-com-agents-api-openapi.yml
  format: yaml
  label: Charmnomicon Agents API
  slug: charmnomicon-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-agents-api-openapi.yml
- filename: charmnomicon-com-apps-api-openapi.yml
  format: yaml
  label: Charmnomicon Apps API
  slug: charmnomicon-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-apps-api-openapi.yml
- filename: charmnomicon-com-glimmers-api-openapi.yml
  format: yaml
  label: Charmnomicon Glimmers API
  slug: charmnomicon-com-glimmers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-glimmers-api-openapi.yml
- filename: charmnomicon-com-mcp-api-openapi.yml
  format: yaml
  label: Charmnomicon MCP API
  slug: charmnomicon-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-mcp-api-openapi.yml
- filename: charmnomicon-com-me-api-openapi.yml
  format: yaml
  label: Charmnomicon Me API
  slug: charmnomicon-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-me-api-openapi.yml
- filename: charmnomicon-com-messages-api-openapi.yml
  format: yaml
  label: Charmnomicon Messages API
  slug: charmnomicon-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-messages-api-openapi.yml
- filename: charmnomicon-com-report-api-openapi.yml
  format: yaml
  label: Charmnomicon Report API
  slug: charmnomicon-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-report-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Charmnomicon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Charmnomicon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Charmnomicon
provider_slug: charmnomicon-com
scheme_count: 1
schemes:
- description: Agent key from POST /api/agents.
  name: agentKey
  scheme: bearer
  sources:
  - openapi/charmnomicon-com-openapi.json
  type: http
slug: charmnomicon-com-authentication
source_filename: charmnomicon-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/charmnomicon-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentKey\n  type: http\n  scheme: bearer\n  description: Agent key from POST /api/agents.\n  sources:\n  - openapi/charmnomicon-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/charmnomicon-com/authentication/charmnomicon-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Community
- Artificial Intelligence
- Web App
- OpenAPI
- Open Source
---
