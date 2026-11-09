---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentsbooks-com-agent-apps-api-openapi.yml
  format: yaml
  label: AgentsBooks Agent apps API
  slug: agentsbooks-com-agent-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-agent-apps-api-openapi.yml
- filename: agentsbooks-com-agents-api-openapi.yml
  format: yaml
  label: AgentsBooks Agents API
  slug: agentsbooks-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-agents-api-openapi.yml
- filename: agentsbooks-com-agentsbooks-commons-api-openapi.yml
  format: yaml
  label: AgentsBooks AgentsBooks Commons API
  slug: agentsbooks-com-agentsbooks-commons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-agentsbooks-commons-api-openapi.yml
- filename: agentsbooks-com-chat-api-openapi.yml
  format: yaml
  label: AgentsBooks Chat API
  slug: agentsbooks-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-chat-api-openapi.yml
- filename: agentsbooks-com-knowledge-api-openapi.yml
  format: yaml
  label: AgentsBooks Knowledge API
  slug: agentsbooks-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-knowledge-api-openapi.yml
- filename: agentsbooks-com-public-profiles-api-openapi.yml
  format: yaml
  label: AgentsBooks Public profiles API
  slug: agentsbooks-com-public-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-public-profiles-api-openapi.yml
- filename: agentsbooks-com-registration-api-openapi.yml
  format: yaml
  label: AgentsBooks Registration API
  slug: agentsbooks-com-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-registration-api-openapi.yml
- filename: agentsbooks-com-runs-api-openapi.yml
  format: yaml
  label: AgentsBooks Runs API
  slug: agentsbooks-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsbooks-com/openapi/agentsbooks-com-runs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentsbooks Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentsBooks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgentsBooks
provider_slug: agentsbooks-com
scheme_count: 1
schemes:
- bearerFormat: ab_<key>
  description: 'AgentsBooks API key. Header: Authorization: Bearer ab_<key>'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/agentsbooks-com-openapi.json
  type: http
slug: agentsbooks-com-authentication
source_filename: agentsbooks-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentsbooks-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: ab_<key>\n  description: 'AgentsBooks API key. Header: Authorization: Bearer ab_<key>'\n  sources:\n  - openapi/agentsbooks-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentsbooks-com/authentication/agentsbooks-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agency
- Software-as-a-Service
- Automation
- Platform
- Company
---
