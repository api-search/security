---
api_key_in: []
api_specs:
- filename: nscale-chat-api-openapi.yml
  format: yaml
  label: Nscale Chat API
  slug: nscale-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-chat-api-openapi.yml
- filename: nscale-completions-api-openapi.yml
  format: yaml
  label: Nscale Completions API
  slug: nscale-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-completions-api-openapi.yml
- filename: nscale-embeddings-api-openapi.yml
  format: yaml
  label: Nscale Embeddings API
  slug: nscale-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-embeddings-api-openapi.yml
- filename: nscale-images-api-openapi.yml
  format: yaml
  label: Nscale Images API
  slug: nscale-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-images-api-openapi.yml
- filename: nscale-models-api-openapi.yml
  format: yaml
  label: Nscale Models API
  slug: nscale-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nscale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nscale
provider_slug: nscale
scheme_count: 1
schemes:
- description: 'Nscale API key issued from the console, sent as `Authorization: Bearer $NSCALE_API_KEY`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nscale-openapi.yml
  type: http
slug: nscale-authentication
source_filename: nscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nscale-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Nscale API key issued from the console, sent as `Authorization: Bearer $NSCALE_API_KEY`.'\n  sources:\n  - openapi/nscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/authentication/nscale-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- GPU
- Inference
- Serverless
- Cloud Compute
---
