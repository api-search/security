---
api_key_in: []
api_specs:
- filename: runpod-billing-api-openapi.yml
  format: yaml
  label: RunPod Billing API
  slug: runpod-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-billing-api-openapi.yml
- filename: runpod-containerregistryauth-api-openapi.yml
  format: yaml
  label: RunPod Containerregistryauth API
  slug: runpod-containerregistryauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-containerregistryauth-api-openapi.yml
- filename: runpod-docs-api-openapi.yml
  format: yaml
  label: RunPod Docs API
  slug: runpod-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-docs-api-openapi.yml
- filename: runpod-endpoints-api-openapi.yml
  format: yaml
  label: RunPod Endpoints API
  slug: runpod-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-endpoints-api-openapi.yml
- filename: runpod-networkvolumes-api-openapi.yml
  format: yaml
  label: RunPod Networkvolumes API
  slug: runpod-networkvolumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-networkvolumes-api-openapi.yml
- filename: runpod-openapi-json-api-openapi.yml
  format: yaml
  label: RunPod Openapi.json API
  slug: runpod-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-openapi-json-api-openapi.yml
- filename: runpod-pods-api-openapi.yml
  format: yaml
  label: RunPod Pods API
  slug: runpod-pods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-pods-api-openapi.yml
- filename: runpod-templates-api-openapi.yml
  format: yaml
  label: RunPod Templates API
  slug: runpod-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/openapi/runpod-templates-api-openapi.yml
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
