---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deepskyai-com-compliance-api-openapi.yml
  format: yaml
  label: Deepsky Compliance API
  slug: deepskyai-com-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-compliance-api-openapi.yml
- filename: deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
  format: yaml
  label: Deepsky Deepsky Aviation Agent API
  slug: deepskyai-com-deepsky-aviation-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
- filename: deepskyai-com-mcp-api-openapi.yml
  format: yaml
  label: Deepsky MCP API
  slug: deepskyai-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-mcp-api-openapi.yml
- filename: deepskyai-com-search-api-openapi.yml
  format: yaml
  label: Deepsky Search API
  slug: deepskyai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-search-api-openapi.yml
- filename: deepskyai-com-skills-api-openapi.yml
  format: yaml
  label: Deepsky Skills API
  slug: deepskyai-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-skills-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Deepsky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepsky secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deepsky
provider_slug: deepskyai-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Supabase user JWT. Contact admin@deepskyai.com for access.
  name: supabaseJwt
  scheme: bearer
  sources:
  - openapi/deepskyai-com-openapi.json
  type: http
slug: deepskyai-com-authentication
source_filename: deepskyai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/deepskyai-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: supabaseJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Supabase user JWT. Contact admin@deepskyai.com for access.\n  sources:\n  - openapi/deepskyai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/deepskyai-com/authentication/deepskyai-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Aviation
- Artificial Intelligence
- Automation
- Documentation
- Compliance
- Company
---
