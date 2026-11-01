---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lamini-embeddings-api-openapi.yml
  format: yaml
  label: Lamini Embeddings API
  slug: lamini-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-embeddings-api-openapi.yml
- filename: lamini-classifier-api-openapi.yml
  format: yaml
  label: Lamini Classifier API
  slug: lamini-classifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-classifier-api-openapi.yml
- filename: lamini-completions-api-openapi.yml
  format: yaml
  label: Lamini Completions API
  slug: lamini-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-completions-api-openapi.yml
- filename: lamini-memory-rag-api-openapi.yml
  format: yaml
  label: Lamini memory rag API
  slug: lamini-memory-rag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-memory-rag-api-openapi.yml
- filename: lamini-model-management-api-openapi.yml
  format: yaml
  label: Lamini model management API
  slug: lamini-model-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-model-management-api-openapi.yml
- filename: lamini-train-api-openapi.yml
  format: yaml
  label: Lamini Train API
  slug: lamini-train-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-train-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lamini Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lamini secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lamini
provider_slug: lamini
scheme_count: 1
schemes:
- description: 'Lamini platform API key passed as Authorization: Bearer <API_KEY>. Requests may also include a Lamini-Version header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lamini-openapi.yml
  type: http
slug: lamini-authentication
source_filename: lamini-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lamini-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Lamini platform API key passed as Authorization: Bearer <API_KEY>. Requests\n    may also include a Lamini-Version header.'\n  sources:\n  - openapi/lamini-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lamini/authentication/lamini-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Fine-Tuning
- Memory Tuning
- Inference
---
