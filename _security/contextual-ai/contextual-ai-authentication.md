---
api_key_in: []
api_specs:
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agents API
  slug: contextual-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agent Query API
  slug: contextual-ai-agent-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Datastores & Documents API
  slug: contextual-ai-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Generate API
  slug: contextual-ai-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Rerank API
  slug: contextual-ai-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Parse API
  slug: contextual-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI LMUnit Evaluation API
  slug: contextual-ai-lmunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Contextual Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contextual AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contextual AI
provider_slug: contextual-ai
scheme_count: 1
schemes:
- description: Contextual AI API key supplied as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contextual-ai-openapi.yml
  type: http
slug: contextual-ai-authentication
source_filename: contextual-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contextual-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Contextual AI API key supplied as a Bearer token.\n  sources:\n  - openapi/contextual-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/authentication/contextual-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- RAG
- LLM
- Grounded Language Model
- Enterprise
---
