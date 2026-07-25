---
api_key_in: []
api_specs:
- filename: ucsd-audio-api-openapi.yml
  format: yaml
  label: University of California, San Diego audio API
  slug: ucsd-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-audio-api-openapi.yml
- filename: ucsd-chat-api-openapi.yml
  format: yaml
  label: University of California, San Diego chat API
  slug: ucsd-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-chat-api-openapi.yml
- filename: ucsd-completions-api-openapi.yml
  format: yaml
  label: University of California, San Diego completions API
  slug: ucsd-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-completions-api-openapi.yml
- filename: ucsd-embeddings-api-openapi.yml
  format: yaml
  label: University of California, San Diego embeddings API
  slug: ucsd-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-embeddings-api-openapi.yml
- filename: ucsd-images-api-openapi.yml
  format: yaml
  label: University of California, San Diego images API
  slug: ucsd-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-images-api-openapi.yml
- filename: ucsd-models-api-openapi.yml
  format: yaml
  label: University of California, San Diego models API
  slug: ucsd-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ucsd Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of California, San Diego secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of California, San Diego
provider_slug: ucsd
scheme_count: 1
schemes:
- description: Issued TritonAI API key passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ucsd-tritonai.yaml
  type: http
slug: ucsd-authentication
source_filename: ucsd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ucsd-tritonai.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Issued TritonAI API key passed as a Bearer token.\n  sources:\n  - openapi/ucsd-tritonai.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/authentication/ucsd-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- United States
- California
---
