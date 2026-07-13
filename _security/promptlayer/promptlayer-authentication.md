---
api_key_in:
- header
api_specs:
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Request Logging & Tracking API
  slug: request-logging-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Prompt Registry & Templates API
  slug: prompt-registry-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Evaluations & Datasets API
  slug: evaluations-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Spans & Traces API
  slug: spans-traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Promptlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: PromptLayer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PromptLayer
provider_slug: promptlayer
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/promptlayer-openapi.yml
  type: apiKey
slug: promptlayer-authentication
source_filename: promptlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/promptlayer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/promptlayer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/authentication/promptlayer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Prompt Engineering
- Prompt Management
- Observability
- Evaluation
---
