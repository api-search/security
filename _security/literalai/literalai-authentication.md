---
api_key_in:
- header
api_specs:
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Threads & Steps API
  slug: threads-steps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Generations API
  slug: generations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Experiments API
  slug: experiments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Prompts API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Scores API
  slug: scores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Literalai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Literal AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Literal AI
provider_slug: literalai
scheme_count: 1
schemes:
- description: Project API key from the Literal AI dashboard, supplied via the LITERAL_API_KEY environment variable in the SDKs.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/literalai-openapi.yml
  type: apiKey
slug: literalai-authentication
source_filename: literalai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/literalai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Project API key from the Literal AI dashboard, supplied via the LITERAL_API_KEY\n    environment variable in the SDKs.\n  sources:\n  - openapi/literalai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/authentication/literalai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Observability
- Evaluation
- Monitoring
---
