---
api_key_in: []
api_specs:
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: prompt-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Recordings & Sessions API
  slug: recordings-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Cases & Datasets API
  slug: test-cases-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Runs & Evaluations API
  slug: test-runs-evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freeplay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freeplay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freeplay
provider_slug: freeplay
scheme_count: 1
schemes:
- description: Authenticate requests using your Freeplay API key as a Bearer token in the Authorization header. API keys are managed at https://app.freeplay.ai/settings/api-access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freeplay-openapi.yml
  type: http
slug: freeplay-authentication
source_filename: freeplay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freeplay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate requests using your Freeplay API key as a Bearer token in the Authorization\n    header. API keys are managed at https://app.freeplay.ai/settings/api-access.\n  sources:\n  - openapi/freeplay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/authentication/freeplay-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
