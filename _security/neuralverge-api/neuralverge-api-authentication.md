---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neuralverge-api-ai-agents-api-openapi.yml
  format: yaml
  label: NeuralVerge API AI Agents API
  slug: neuralverge-api-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/openapi/neuralverge-api-ai-agents-api-openapi.yml
- filename: neuralverge-api-ai-extract-api-openapi.yml
  format: yaml
  label: NeuralVerge API AI Extract API
  slug: neuralverge-api-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/openapi/neuralverge-api-ai-extract-api-openapi.yml
- filename: neuralverge-api-ai-research-api-openapi.yml
  format: yaml
  label: NeuralVerge API AI Research API
  slug: neuralverge-api-ai-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/openapi/neuralverge-api-ai-research-api-openapi.yml
- filename: neuralverge-api-data-sources-api-openapi.yml
  format: yaml
  label: NeuralVerge API Data Sources API
  slug: neuralverge-api-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/openapi/neuralverge-api-data-sources-api-openapi.yml
- filename: neuralverge-api-search-api-openapi.yml
  format: yaml
  label: NeuralVerge API Search API
  slug: neuralverge-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/openapi/neuralverge-api-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Neuralverge Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeuralVerge API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NeuralVerge API
provider_slug: neuralverge-api
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/neuralverge-api-openapi.json
  type: http
slug: neuralverge-api-authentication
source_filename: neuralverge-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/neuralverge-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/neuralverge-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuralverge-api/refs/heads/main/authentication/neuralverge-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Company Data
- People Data
- Contact Enrichment
- Email Finder
- Email Verification
- Phone Lookup
- corporate registries
- KYB / compliance
- Web Extraction
- Deep Research
- Web Search
- LinkedIn data
- MCP
- AI Agents
- A2A
- Data Enrichment
---
