---
api_key_in:
- header
api_specs:
- filename: exa-search-api-openapi.yml
  format: yaml
  label: Exa Search API
  slug: exa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-search-api-openapi.yml
- filename: exa-research-api-openapi.yml
  format: yaml
  label: Exa Research API
  slug: exa-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-research-api-openapi.yml
- filename: exa-monitors-api-openapi.yml
  format: yaml
  label: Exa Monitors API
  slug: exa-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-monitors-api-openapi.yml
- filename: exa-agent-api-openapi.yml
  format: yaml
  label: Exa Agent API
  slug: exa-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-agent-api-openapi.yml
- filename: exa-websets-api-openapi.yml
  format: yaml
  label: Exa Websets API
  slug: exa-websets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-websets-api-openapi.yml
- filename: exa-team-api-openapi.yml
  format: yaml
  label: Exa Team API
  slug: exa-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-team-api-openapi.yml
- filename: exa-team-management-api-openapi.yml
  format: yaml
  label: Exa Team Management API
  slug: exa-team-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-team-management-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Exa Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exa secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Exa
provider_slug: exa-ai
scheme_count: 2
schemes:
- description: 'Pass your Exa API key in the x-api-key header. You can also authenticate with Authorization: Bearer <key>.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/exa-agent-api-openapi.yml
  - openapi/exa-monitors-api-openapi.yml
  - openapi/exa-research-api-openapi.yml
  - openapi/exa-search-api-openapi.yml
  - openapi/exa-team-api-openapi.yml
  - openapi/exa-team-management-api-openapi.yml
  - openapi/exa-websets-api-openapi.yml
  type: apiKey
- description: 'Pass your Exa API key in the x-api-key header. You can also authenticate with Authorization: Bearer <key>.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/exa-agent-api-openapi.yml
  - openapi/exa-monitors-api-openapi.yml
  - openapi/exa-research-api-openapi.yml
  - openapi/exa-search-api-openapi.yml
  - openapi/exa-team-api-openapi.yml
  - openapi/exa-websets-api-openapi.yml
  type: http
slug: exa-ai-authentication
source_filename: exa-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exa-agent-api-openapi.yml, openapi/exa-monitors-api-openapi.yml, openapi/exa-research-api-openapi.yml,\n  openapi/exa-search-api-openapi.yml, openapi/exa-team-api-openapi.yml, openapi/exa-team-management-api-openapi.yml,\n  openapi/exa-websets-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Pass your Exa API key in the x-api-key header. You can also authenticate with\n    Authorization: Bearer <key>.'\n  sources:\n  - openapi/exa-agent-api-openapi.yml\n  - openapi/exa-monitors-api-openapi.yml\n  - openapi/exa-research-api-openapi.yml\n  - openapi/exa-search-api-openapi.yml\n  - openapi/exa-team-api-openapi.yml\n  - openapi/exa-team-management-api-openapi.yml\n  - openapi/exa-websets-api-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Pass your Exa API key in\
  \ the x-api-key header. You can also authenticate with\n    Authorization: Bearer <key>.'\n  sources:\n  - openapi/exa-agent-api-openapi.yml\n  - openapi/exa-monitors-api-openapi.yml\n  - openapi/exa-research-api-openapi.yml\n  - openapi/exa-search-api-openapi.yml\n  - openapi/exa-team-api-openapi.yml\n  - openapi/exa-websets-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/authentication/exa-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Search
- Web Search
- Neural Search
- LLM
- Agents
- Research
- Websets
---
