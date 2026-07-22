---
api_key_in: []
api_specs:
- filename: uselemma-platform-api-openapi-original.json
  format: json
  label: Lemma Platform API
  slug: uselemma-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uselemma/refs/heads/main/openapi/uselemma-platform-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uselemma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemma
provider_slug: uselemma
scheme_count: 1
schemes:
- name: bearerAuth
  notes: 'The bearer token is a project API key with prefix lma_, created in Lemma project settings (platform.uselemma.ai) and shown only once at creation. SDK clients read it from LEMMA_API_KEY (with LEMMA_PROJECT_ID, prefix proj_, selecting the project). The same key authenticates the Platform API, trace ingest, and the remote MCP server at https://api.uselemma.ai/mcp (Authorization: Bearer header). Missing credentials return 401; the entire api.uselemma.ai host is authenticated.'
  scheme: bearer
  sources:
  - openapi/uselemma-platform-api-openapi-original.json
  type: http
slug: uselemma-authentication
source_filename: uselemma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/uselemma-platform-api-openapi-original.json\ndocs: https://docs.uselemma.ai/tracing/instrumentation/setup\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/uselemma-platform-api-openapi-original.json\n  notes: >-\n    The bearer token is a project API key with prefix lma_, created in Lemma\n    project settings (platform.uselemma.ai) and shown only once at creation.\n    SDK clients read it from LEMMA_API_KEY (with LEMMA_PROJECT_ID, prefix\n    proj_, selecting the project). The same key authenticates the Platform\n    API, trace ingest, and the remote MCP server at\n    https://api.uselemma.ai/mcp (Authorization: Bearer header). Missing\n    credentials return 401; the entire api.uselemma.ai host is authenticated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uselemma/refs/heads/main/authentication/uselemma-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Observability
- Monitoring
- Tracing
- Developer Tools
- B2B
---
