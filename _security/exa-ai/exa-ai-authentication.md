---
api_key_in:
- header
api_specs:
- filename: exa-ai-agent-api-openapi.yml
  format: yaml
  label: Exa Agent API
  slug: exa-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-agent-api-openapi.yml
- filename: exa-ai-answer-api-openapi.yml
  format: yaml
  label: Exa Answer API
  slug: exa-ai-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-answer-api-openapi.yml
- filename: exa-ai-contents-api-openapi.yml
  format: yaml
  label: Exa Contents API
  slug: exa-ai-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-contents-api-openapi.yml
- filename: exa-ai-enrichments-api-openapi.yml
  format: yaml
  label: Exa Enrichments API
  slug: exa-ai-enrichments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-enrichments-api-openapi.yml
- filename: exa-ai-events-api-openapi.yml
  format: yaml
  label: Exa Events API
  slug: exa-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-events-api-openapi.yml
- filename: exa-ai-imports-api-openapi.yml
  format: yaml
  label: Exa Imports API
  slug: exa-ai-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-imports-api-openapi.yml
- filename: exa-ai-items-api-openapi.yml
  format: yaml
  label: Exa Items API
  slug: exa-ai-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-items-api-openapi.yml
- filename: exa-ai-monitors-api-openapi.yml
  format: yaml
  label: Exa Monitors API
  slug: exa-ai-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-monitors-api-openapi.yml
- filename: exa-ai-monitors-runs-api-openapi.yml
  format: yaml
  label: Exa Monitors Runs API
  slug: exa-ai-monitors-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-monitors-runs-api-openapi.yml
- filename: exa-ai-research-api-openapi.yml
  format: yaml
  label: Exa Research API
  slug: exa-ai-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-research-api-openapi.yml
- filename: exa-ai-runs-api-openapi.yml
  format: yaml
  label: Exa Runs API
  slug: exa-ai-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-runs-api-openapi.yml
- filename: exa-ai-search-api-openapi.yml
  format: yaml
  label: Exa Search API
  slug: exa-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-search-api-openapi.yml
- filename: exa-ai-searches-api-openapi.yml
  format: yaml
  label: Exa Searches API
  slug: exa-ai-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-searches-api-openapi.yml
- filename: exa-ai-team-management-api-openapi.yml
  format: yaml
  label: Exa Team Management API
  slug: exa-ai-team-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-team-management-api-openapi.yml
- filename: exa-ai-teams-api-openapi.yml
  format: yaml
  label: Exa Teams API
  slug: exa-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-teams-api-openapi.yml
- filename: exa-ai-webhooks-api-openapi.yml
  format: yaml
  label: Exa Webhooks API
  slug: exa-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-webhooks-api-openapi.yml
- filename: exa-ai-webhooks-attempts-api-openapi.yml
  format: yaml
  label: Exa Webhooks Attempts API
  slug: exa-ai-webhooks-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-webhooks-attempts-api-openapi.yml
- filename: exa-ai-websets-api-openapi.yml
  format: yaml
  label: Exa Websets API
  slug: exa-ai-websets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-websets-api-openapi.yml
- filename: exa-ai-websets-preview-api-openapi.yml
  format: yaml
  label: Exa Websets Preview API
  slug: exa-ai-websets-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa-ai/refs/heads/main/openapi/exa-ai-websets-preview-api-openapi.yml
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
- Artificial Intelligence
- Search
- Web Search
- Neural Search
- LLM
- Agents
- Research
- Websets
---
