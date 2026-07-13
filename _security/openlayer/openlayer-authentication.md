---
api_key_in: []
api_specs:
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Projects API
  slug: openlayer-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Inference Pipelines API
  slug: openlayer-inference-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Data Stream API
  slug: openlayer-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Commits and Test Results API
  slug: openlayer-commits-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
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
- AI
- Evaluation
- Testing
- Observability
- LLM
- MLOps
---
