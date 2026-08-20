---
api_key_in: []
api_specs:
- filename: openlayer-commits-api-openapi.yml
  format: yaml
  label: Openlayer Commits API
  slug: openlayer-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-commits-api-openapi.yml
- filename: openlayer-data-stream-api-openapi.yml
  format: yaml
  label: Openlayer Data Stream API
  slug: openlayer-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-data-stream-api-openapi.yml
- filename: openlayer-inference-pipelines-api-openapi.yml
  format: yaml
  label: Openlayer Inference Pipelines API
  slug: openlayer-inference-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-inference-pipelines-api-openapi.yml
- filename: openlayer-projects-api-openapi.yml
  format: yaml
  label: Openlayer Projects API
  slug: openlayer-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-projects-api-openapi.yml
- filename: openlayer-storage-api-openapi.yml
  format: yaml
  label: Openlayer Storage API
  slug: openlayer-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-storage-api-openapi.yml
- filename: openlayer-tests-api-openapi.yml
  format: yaml
  label: Openlayer Tests API
  slug: openlayer-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-tests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openlayer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Openlayer
provider_slug: openlayer
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: Pass your Openlayer API key as a Bearer token in the Authorization header.
  name: api_key
  scheme: bearer
  sources:
  - openapi/openlayer-openapi.yml
  type: http
slug: openlayer-authentication
source_filename: openlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openlayer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: Pass your Openlayer API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/openlayer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/authentication/openlayer-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Evaluation
- Testing
- Observability
- LLM
- MLOps
---
