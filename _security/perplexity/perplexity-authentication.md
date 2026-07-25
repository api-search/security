---
api_key_in: []
api_specs:
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Async Chat Completions API
  slug: async-chat-completions-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Responses API
  slug: responses-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-agent-api-openapi.yml
  format: yaml
  label: Perplexity Agent API
  slug: perplexity-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-agent-api-openapi.yml
- filename: perplexity-async-api-openapi.yml
  format: yaml
  label: Perplexity Async API
  slug: perplexity-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-async-api-openapi.yml
- filename: perplexity-contextualizedembeddings-api-openapi.yml
  format: yaml
  label: Perplexity Contextualizedembeddings API
  slug: perplexity-contextualizedembeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-contextualizedembeddings-api-openapi.yml
- filename: perplexity-embeddings-api-openapi.yml
  format: yaml
  label: Perplexity Embeddings API
  slug: perplexity-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-embeddings-api-openapi.yml
- filename: perplexity-models-api-openapi.yml
  format: yaml
  label: Perplexity Models API
  slug: perplexity-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-models-api-openapi.yml
- filename: perplexity-search-api-openapi.yml
  format: yaml
  label: Perplexity Search API
  slug: perplexity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-search-api-openapi.yml
- filename: perplexity-sonar-api-openapi.yml
  format: yaml
  label: Perplexity Sonar API
  slug: perplexity-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-sonar-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Perplexity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perplexity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perplexity
provider_slug: perplexity
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/perplexity-openapi.json
  type: http
slug: perplexity-authentication
source_filename: perplexity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/perplexity-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/perplexity-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/authentication/perplexity-authentication.yml
summary_line: http · 1 scheme
tags: []
---
