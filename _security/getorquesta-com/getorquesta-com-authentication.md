---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getorquesta-com-agent-mesh-api-openapi.yml
  format: yaml
  label: Orquesta Agent Mesh API
  slug: getorquesta-com-agent-mesh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-agent-mesh-api-openapi.yml
- filename: getorquesta-com-agents-api-openapi.yml
  format: yaml
  label: Orquesta Agents API
  slug: getorquesta-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-agents-api-openapi.yml
- filename: getorquesta-com-batuta-llm-api-openapi.yml
  format: yaml
  label: Orquesta Batuta LLM API
  slug: getorquesta-com-batuta-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-batuta-llm-api-openapi.yml
- filename: getorquesta-com-logs-api-openapi.yml
  format: yaml
  label: Orquesta Logs API
  slug: getorquesta-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-logs-api-openapi.yml
- filename: getorquesta-com-projects-api-openapi.yml
  format: yaml
  label: Orquesta Projects API
  slug: getorquesta-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-projects-api-openapi.yml
- filename: getorquesta-com-prompts-api-openapi.yml
  format: yaml
  label: Orquesta Prompts API
  slug: getorquesta-com-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-prompts-api-openapi.yml
- filename: getorquesta-com-users-api-openapi.yml
  format: yaml
  label: Orquesta Users API
  slug: getorquesta-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-users-api-openapi.yml
- filename: getorquesta-com-workstreams-api-openapi.yml
  format: yaml
  label: Orquesta Workstreams API
  slug: getorquesta-com-workstreams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getorquesta-com/openapi/getorquesta-com-workstreams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Orquesta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orquesta secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orquesta
provider_slug: getorquesta-com
scheme_count: 2
schemes:
- bearerFormat: orquesta-token (oak_|oclt_|oat_)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/getorquesta-com-openapi.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/getorquesta-com-openapi.json
  type: apiKey
slug: getorquesta-com-authentication
source_filename: getorquesta-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getorquesta-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: orquesta-token (oak_|oclt_|oat_)\n  sources:\n  - openapi/getorquesta-com-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/getorquesta-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getorquesta-com/authentication/getorquesta-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Automation
- Business
- Platform
- Orchestrator
---
