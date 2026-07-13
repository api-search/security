---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Hugging Face Inference API
  slug: hugging-face-inference-api
  spec_type: OpenAPI
  url: https://huggingface.co/api-inference/openapi.json
- filename: openapi.json
  format: json
  label: Hugging Face Hub API
  slug: hugging-face-hub-api
  spec_type: OpenAPI
  url: https://huggingface.co/.well-known/openapi.json
- filename: hugging-face-inference-endpoints-api.yml
  format: yaml
  label: Hugging Face Inference Endpoints API
  slug: hugging-face-inference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-inference-endpoints-api.yml
- filename: hugging-face-inference-providers-api.yml
  format: yaml
  label: Hugging Face Inference Providers API
  slug: hugging-face-inference-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-inference-providers-api.yml
- filename: openapi.json
  format: json
  label: Hugging Face Dataset Viewer API
  slug: hugging-face-dataset-viewer-api
  spec_type: OpenAPI
  url: https://datasets-server.huggingface.co/openapi.json
- filename: hugging-face-text-generation-inference-api.yml
  format: yaml
  label: Hugging Face Text Generation Inference API
  slug: hugging-face-text-generation-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-text-generation-inference-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hugging Face Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hugging Face secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hugging Face
provider_slug: hugging-face
scheme_count: 1
schemes:
- bearerFormat: HF Token
  description: Optional Hugging Face API token. Required for private and gated datasets.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hugging-face-dataset-viewer-api.yml
  - openapi/hugging-face-hub-api.yml
  - openapi/hugging-face-inference-api.yml
  - openapi/hugging-face-inference-endpoints-api.yml
  - openapi/hugging-face-inference-providers-api.yml
  - openapi/hugging-face-text-generation-inference-api.yml
  type: http
slug: hugging-face-authentication
source_filename: hugging-face-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hugging-face-dataset-viewer-api.yml, openapi/hugging-face-hub-api.yml, openapi/hugging-face-inference-api.yml,\n  openapi/hugging-face-inference-endpoints-api.yml, openapi/hugging-face-inference-providers-api.yml,\n  openapi/hugging-face-text-generation-inference-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: HF Token\n  description: Optional Hugging Face API token. Required for private and gated datasets.\n  sources:\n  - openapi/hugging-face-dataset-viewer-api.yml\n  - openapi/hugging-face-hub-api.yml\n  - openapi/hugging-face-inference-api.yml\n  - openapi/hugging-face-inference-endpoints-api.yml\n  - openapi/hugging-face-inference-providers-api.yml\n  - openapi/hugging-face-text-generation-inference-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/authentication/hugging-face-authentication.yml
summary_line: http · 1 scheme
tags: []
---
