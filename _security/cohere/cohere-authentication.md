---
api_key_in: []
api_specs:
- filename: cohere-chat-api-openapi.yml
  format: yaml
  label: Cohere Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-chat-api-openapi.yml
- filename: cohere-embed-api-openapi.yml
  format: yaml
  label: Cohere Embed API
  slug: embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-embed-api-openapi.yml
- filename: cohere-rerank-api-openapi.yml
  format: yaml
  label: Cohere Rerank API
  slug: rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-rerank-api-openapi.yml
- filename: cohere-classify-api-openapi.yml
  format: yaml
  label: Cohere Classify API
  slug: classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-classify-api-openapi.yml
- filename: cohere-embed-jobs-api-openapi.yml
  format: yaml
  label: Cohere Embed Jobs API
  slug: embed-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-embed-jobs-api-openapi.yml
- filename: cohere-datasets-api-openapi.yml
  format: yaml
  label: Cohere Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-datasets-api-openapi.yml
- filename: cohere-models-api-openapi.yml
  format: yaml
  label: Cohere Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-models-api-openapi.yml
- filename: cohere-tokenize-api-openapi.yml
  format: yaml
  label: Cohere Tokenize API
  slug: tokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-tokenize-api-openapi.yml
- filename: cohere-detokenize-api-openapi.yml
  format: yaml
  label: Cohere Detokenize API
  slug: detokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-detokenize-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cohere Authentication
name_suffix: Authentication
oauth_flows: []
overview: cohere secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: cohere
provider_slug: cohere
scheme_count: 1
schemes:
- description: Bearer authentication using a Cohere API key. Pass the API key in the Authorization header as Bearer <token>.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cohere-chat-api-openapi.yml
  - openapi/cohere-classify-api-openapi.yml
  - openapi/cohere-datasets-api-openapi.yml
  - openapi/cohere-detokenize-api-openapi.yml
  - openapi/cohere-embed-api-openapi.yml
  - openapi/cohere-embed-jobs-api-openapi.yml
  - openapi/cohere-models-api-openapi.yml
  - openapi/cohere-rerank-api-openapi.yml
  - openapi/cohere-tokenize-api-openapi.yml
  type: http
slug: cohere-authentication
source_filename: cohere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cohere-chat-api-openapi.yml, openapi/cohere-classify-api-openapi.yml, openapi/cohere-datasets-api-openapi.yml,\n  openapi/cohere-detokenize-api-openapi.yml, openapi/cohere-embed-api-openapi.yml, openapi/cohere-embed-jobs-api-openapi.yml,\n  openapi/cohere-models-api-openapi.yml, openapi/cohere-rerank-api-openapi.yml, openapi/cohere-tokenize-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication using a Cohere API key. Pass the API key in the Authorization\n    header as Bearer <token>.\n  sources:\n  - openapi/cohere-chat-api-openapi.yml\n  - openapi/cohere-classify-api-openapi.yml\n  - openapi/cohere-datasets-api-openapi.yml\n  - openapi/cohere-detokenize-api-openapi.yml\n  - openapi/cohere-embed-api-openapi.yml\n  - openapi/cohere-embed-jobs-api-openapi.yml\n  - openapi/cohere-models-api-openapi.yml\n  - openapi/cohere-rerank-api-openapi.yml\n\
  \  - openapi/cohere-tokenize-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/authentication/cohere-authentication.yml
summary_line: http · 1 scheme
tags: []
---
