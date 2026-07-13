---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: RunPod REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://rest.runpod.io/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runpod Authentication
name_suffix: Authentication
oauth_flows: []
overview: RunPod secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RunPod
provider_slug: runpod
scheme_count: 1
schemes:
- description: Runpod API key supplied as a bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runpod-openapi.yml
  type: http
slug: runpod-authentication
source_filename: runpod-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runpod-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Runpod API key supplied as a bearer token.\n  sources:\n  - openapi/runpod-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/authentication/runpod-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Cloud
- Compute
- GPU
- Inference
- Machine Learning
- Serverless
---
