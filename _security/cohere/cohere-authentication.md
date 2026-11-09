---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cohere-chat-api-openapi.yml
  format: yaml
  label: Cohere Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-chat-api-openapi.yml
- filename: cohere-embed-api-openapi.yml
  format: yaml
  label: Cohere Embed API
  slug: embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-embed-api-openapi.yml
- filename: cohere-rerank-api-openapi.yml
  format: yaml
  label: Cohere Rerank API
  slug: rerank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-rerank-api-openapi.yml
- filename: cohere-classify-api-openapi.yml
  format: yaml
  label: Cohere Classify API
  slug: classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-classify-api-openapi.yml
- filename: cohere-datasets-api-openapi.yml
  format: yaml
  label: Cohere Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-datasets-api-openapi.yml
- filename: cohere-models-api-openapi.yml
  format: yaml
  label: Cohere Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-models-api-openapi.yml
- filename: cohere-tokenize-api-openapi.yml
  format: yaml
  label: Cohere Tokenize API
  slug: tokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-tokenize-api-openapi.yml
- filename: cohere-detokenize-api-openapi.yml
  format: yaml
  label: Cohere Detokenize API
  slug: detokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-detokenize-api-openapi.yml
- filename: cohere-batches-api-openapi.yml
  format: yaml
  label: Cohere Batches API
  slug: cohere-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-batches-api-openapi.yml
- filename: cohere-check-api-key-api-openapi.yml
  format: yaml
  label: Cohere Check Api Key API
  slug: cohere-check-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-check-api-key-api-openapi.yml
- filename: cohere-connectors-api-openapi.yml
  format: yaml
  label: Cohere Connectors API
  slug: cohere-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-connectors-api-openapi.yml
- filename: cohere-embedjobs-api-openapi.yml
  format: yaml
  label: Cohere Embed Jobs API
  slug: cohere-embedjobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-embedjobs-api-openapi.yml
- filename: cohere-finetuning-api-openapi.yml
  format: yaml
  label: Cohere /finetuning API
  slug: cohere-finetuning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-finetuning-api-openapi.yml
- filename: cohere-generate-api-openapi.yml
  format: yaml
  label: Cohere Generate API
  slug: cohere-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-generate-api-openapi.yml
- filename: cohere-parse-api-openapi.yml
  format: yaml
  label: Cohere Parse API
  slug: cohere-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-parse-api-openapi.yml
- filename: cohere-summarize-api-openapi.yml
  format: yaml
  label: Cohere Summarize API
  slug: cohere-summarize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-summarize-api-openapi.yml
- filename: cohere-transcriptions-api-openapi.yml
  format: yaml
  label: Cohere Transcriptions API
  slug: cohere-transcriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohere/openapi/cohere-transcriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cohere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cohere secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cohere
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
source_yaml_url: https://artifacts.apis.io/cohere/authentication/cohere-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Natural Language Processing
- Embeddings
- Vector Search
- LLM
- Canada
- Foundation Models
---
