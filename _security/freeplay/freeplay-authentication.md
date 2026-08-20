---
api_key_in: []
api_specs:
- filename: freeplay-agents-api-openapi.yml
  format: yaml
  label: Freeplay Agents API
  slug: freeplay-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-agents-api-openapi.yml
- filename: freeplay-completions-api-openapi.yml
  format: yaml
  label: Freeplay Completions API
  slug: freeplay-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-completions-api-openapi.yml
- filename: freeplay-datasets-api-openapi.yml
  format: yaml
  label: Freeplay Datasets API
  slug: freeplay-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-datasets-api-openapi.yml
- filename: freeplay-feedback-api-openapi.yml
  format: yaml
  label: Freeplay Feedback API
  slug: freeplay-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-feedback-api-openapi.yml
- filename: freeplay-projects-api-openapi.yml
  format: yaml
  label: Freeplay Projects API
  slug: freeplay-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-projects-api-openapi.yml
- filename: freeplay-prompt-templates-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: freeplay-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-prompt-templates-api-openapi.yml
- filename: freeplay-search-api-openapi.yml
  format: yaml
  label: Freeplay Search API
  slug: freeplay-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-search-api-openapi.yml
- filename: freeplay-sessions-api-openapi.yml
  format: yaml
  label: Freeplay Sessions API
  slug: freeplay-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-sessions-api-openapi.yml
- filename: freeplay-test-runs-api-openapi.yml
  format: yaml
  label: Freeplay Test Runs API
  slug: freeplay-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-test-runs-api-openapi.yml
- filename: freeplay-traces-api-openapi.yml
  format: yaml
  label: Freeplay Traces API
  slug: freeplay-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-traces-api-openapi.yml
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
- Artificial Intelligence
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
