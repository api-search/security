---
api_key_in: []
api_specs:
- filename: truefoundry-audio-api-openapi.yml
  format: yaml
  label: TrueFoundry Audio API
  slug: truefoundry-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-audio-api-openapi.yml
- filename: truefoundry-batches-api-openapi.yml
  format: yaml
  label: TrueFoundry Batches API
  slug: truefoundry-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-batches-api-openapi.yml
- filename: truefoundry-chat-api-openapi.yml
  format: yaml
  label: TrueFoundry Chat API
  slug: truefoundry-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-chat-api-openapi.yml
- filename: truefoundry-embeddings-api-openapi.yml
  format: yaml
  label: TrueFoundry Embeddings API
  slug: truefoundry-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-embeddings-api-openapi.yml
- filename: truefoundry-files-api-openapi.yml
  format: yaml
  label: TrueFoundry Files API
  slug: truefoundry-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-files-api-openapi.yml
- filename: truefoundry-images-api-openapi.yml
  format: yaml
  label: TrueFoundry Images API
  slug: truefoundry-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-images-api-openapi.yml
- filename: truefoundry-models-api-openapi.yml
  format: yaml
  label: TrueFoundry Models API
  slug: truefoundry-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-models-api-openapi.yml
- filename: truefoundry-moderations-api-openapi.yml
  format: yaml
  label: TrueFoundry Moderations API
  slug: truefoundry-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-moderations-api-openapi.yml
- filename: truefoundry-rerank-api-openapi.yml
  format: yaml
  label: TrueFoundry Rerank API
  slug: truefoundry-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-rerank-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Truefoundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueFoundry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueFoundry
provider_slug: truefoundry
scheme_count: 1
schemes:
- description: TrueFoundry API key (JWT format)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/truefoundry-ai-gateway-openapi.yml
  type: http
slug: truefoundry-authentication
source_filename: truefoundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truefoundry-ai-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: TrueFoundry API key (JWT format)\n  sources:\n  - openapi/truefoundry-ai-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/authentication/truefoundry-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Platform
- Enterprise AI
- Kubernetes
- LLM Gateway
- MLOps
---
