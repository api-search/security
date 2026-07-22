---
api_key_in:
- header
api_specs:
- filename: tako-openapi-original.yml
  format: yaml
  label: Tako Knowledge Search API
  slug: tako-knowledge-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/openapi/tako-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tako Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tako secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tako
provider_slug: tako
scheme_count: 1
schemes:
- applied_to:
  - search
  - answer
  - contents
  - createCard
  - listAnswerAgentRuns
  - createAnswerAgentRun
  - getAnswerAgentRun
  - listRetrievalAgentRuns
  - createRetrievalAgentRun
  - getRetrievalAgentRun
  in: header
  name: apiKey
  parameter_name: X-API-Key
  sources:
  - openapi/tako-openapi-original.yml
  type: apiKey
slug: tako-authentication
source_filename: tako-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tako-openapi-original.yml\ndocs: https://docs.tako.com/documentation/getting-started/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_header: X-API-Key\n  oauth2_flows: []\n  notes: >-\n    Single auth mechanism: a per-environment API key sent in the X-API-Key\n    header. Create keys in the Tako Console (https://tako.com/console/api-keys).\n    A key only authenticates on the host it was issued for. Anonymous calls to\n    key-protected endpoints return 401 (AUTHENTICATION_ERROR). The three\n    /beta/graph/* endpoints are public and unauthenticated.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: X-API-Key\n    sources: [openapi/tako-openapi-original.yml]\n    applied_to:\n      - search\n      - answer\n      - contents\n      - createCard\n      - listAnswerAgentRuns\n      - createAnswerAgentRun\n      - getAnswerAgentRun\n      - listRetrievalAgentRuns\n\
  \      - createRetrievalAgentRun\n      - getRetrievalAgentRun\npublic_operations:\n  - graphSearch\n  - graphRelated\n  - graphNode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/authentication/tako-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Data
- Search
- Answer Engine
- Financial Data
- Knowledge Graph
- Agents
- MCP
- Data Visualization
---
