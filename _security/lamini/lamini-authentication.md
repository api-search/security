---
api_key_in: []
api_specs:
- filename: lamini-classify-api-openapi.yml
  format: yaml
  label: Lamini Classify API
  slug: lamini-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-classify-api-openapi.yml
- filename: lamini-embeddings-api-openapi.yml
  format: yaml
  label: Lamini Embeddings API
  slug: lamini-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-embeddings-api-openapi.yml
- filename: lamini-fine-tuning-api-openapi.yml
  format: yaml
  label: Lamini Fine-Tuning API
  slug: lamini-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-fine-tuning-api-openapi.yml
- filename: lamini-inference-api-openapi.yml
  format: yaml
  label: Lamini Inference API
  slug: lamini-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-inference-api-openapi.yml
- filename: lamini-platform-api-openapi.yml
  format: yaml
  label: Lamini Platform API
  slug: lamini-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/authentication/lamini-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Fine-Tuning
- Memory Tuning
- Inference
---
