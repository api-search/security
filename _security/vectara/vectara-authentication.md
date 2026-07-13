---
api_key_in:
- header
api_specs:
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara REST API
  slug: vectara-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Corpora API
  slug: vectara-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Indexing API
  slug: vectara-indexing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Query API
  slug: vectara-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Agents API
  slug: vectara-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vectara Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vectara secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vectara
provider_slug: vectara
scheme_count: 2
schemes:
- description: Vectara API key passed in the `x-api-key` header.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/vectara-openapi.yml
  type: apiKey
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  sources:
  - openapi/vectara-openapi.yml
  type: oauth2
slug: vectara-authentication
source_filename: vectara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vectara-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Vectara API key passed in the `x-api-key` header.\n  sources:\n  - openapi/vectara-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 client credentials flow.\n  sources:\n  - openapi/vectara-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/authentication/vectara-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI
- Agents
- Corpora
- Embeddings
- Enterprise Search
- Generative AI
- Grounded Generation
- Hallucination Detection
- LLM
- MCP
- RAG
- Retrieval
- Search
- Semantic Search
- Vector Search
---
