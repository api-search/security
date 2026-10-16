---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastrouter-audio-api-openapi.yml
  format: yaml
  label: Fastrouter Audio API
  slug: fastrouter-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-audio-api-openapi.yml
- filename: fastrouter-batches-api-openapi.yml
  format: yaml
  label: Fastrouter Batches API
  slug: fastrouter-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-batches-api-openapi.yml
- filename: fastrouter-embeddings-api-openapi.yml
  format: yaml
  label: Fastrouter Embeddings API
  slug: fastrouter-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-embeddings-api-openapi.yml
- filename: fastrouter-files-api-openapi.yml
  format: yaml
  label: Fastrouter Files API
  slug: fastrouter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-files-api-openapi.yml
- filename: fastrouter-generation-api-openapi.yml
  format: yaml
  label: Fastrouter Generation API
  slug: fastrouter-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-generation-api-openapi.yml
- filename: fastrouter-getasyncresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Async Response API
  slug: fastrouter-getasyncresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getasyncresponse-api-openapi.yml
- filename: fastrouter-getprompttoaudioresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Prompt To Audio Response API
  slug: fastrouter-getprompttoaudioresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getprompttoaudioresponse-api-openapi.yml
- filename: fastrouter-images-api-openapi.yml
  format: yaml
  label: Fastrouter Images API
  slug: fastrouter-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-images-api-openapi.yml
- filename: fastrouter-model-api-openapi.yml
  format: yaml
  label: Fastrouter Model API
  slug: fastrouter-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-model-api-openapi.yml
- filename: fastrouter-models-api-openapi.yml
  format: yaml
  label: Fastrouter Models API
  slug: fastrouter-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-models-api-openapi.yml
- filename: fastrouter-moderations-api-openapi.yml
  format: yaml
  label: Fastrouter Moderations API
  slug: fastrouter-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-moderations-api-openapi.yml
- filename: fastrouter-responses-api-openapi.yml
  format: yaml
  label: Fastrouter Responses API
  slug: fastrouter-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-responses-api-openapi.yml
- filename: fastrouter-videos-api-openapi.yml
  format: yaml
  label: Fastrouter Videos API
  slug: fastrouter-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-videos-api-openapi.yml
- filename: fastrouter-chat-completions-api-openapi.yml
  format: yaml
  label: Fastrouter Chat Completions API
  slug: fastrouter-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fastrouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fastrouter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fastrouter
provider_slug: fastrouter
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fastrouter-openapi.json
  type: http
slug: fastrouter-authentication
source_filename: fastrouter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: derived\nsource: openapi/fastrouter-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fastrouter-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/authentication/fastrouter-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- API Gateway
- LLM
- Enterprise
---
