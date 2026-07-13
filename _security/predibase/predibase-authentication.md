---
api_key_in: []
api_specs:
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Inference (OpenAI-Compatible) API
  slug: predibase-inference-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Prompt / Generate API
  slug: predibase-prompt-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Fine-Tuning API
  slug: predibase-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Adapters API
  slug: predibase-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Deployments API
  slug: predibase-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Datasets API
  slug: predibase-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Models API
  slug: predibase-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Batch Inference API
  slug: predibase-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Predibase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Predibase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Predibase
provider_slug: predibase
scheme_count: 1
schemes:
- bearerFormat: Predibase API token
  description: 'Predibase API token sent as Authorization: Bearer <PREDIBASE_API_TOKEN>. Generate a token from Settings in the Predibase console.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/predibase-openapi.yml
  type: http
slug: predibase-authentication
source_filename: predibase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/predibase-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Predibase API token\n  description: 'Predibase API token sent as Authorization: Bearer <PREDIBASE_API_TOKEN>. Generate\n    a token from Settings in the Predibase console.'\n  sources:\n  - openapi/predibase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/authentication/predibase-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Fine-Tuning
- Inference
- LoRA
---
