---
api_key_in: []
api_specs:
- filename: wandb-calls-api-openapi.yml
  format: yaml
  label: Weights and Biases Calls API
  slug: wandb-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-calls-api-openapi.yml
- filename: wandb-costs-api-openapi.yml
  format: yaml
  label: Weights and Biases Costs API
  slug: wandb-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-costs-api-openapi.yml
- filename: wandb-feedback-api-openapi.yml
  format: yaml
  label: Weights and Biases Feedback API
  slug: wandb-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-feedback-api-openapi.yml
- filename: wandb-files-api-openapi.yml
  format: yaml
  label: Weights and Biases Files API
  slug: wandb-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-files-api-openapi.yml
- filename: wandb-objects-api-openapi.yml
  format: yaml
  label: Weights and Biases Objects API
  slug: wandb-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-objects-api-openapi.yml
- filename: wandb-refs-api-openapi.yml
  format: yaml
  label: Weights and Biases Refs API
  slug: wandb-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-refs-api-openapi.yml
- filename: wandb-service-api-openapi.yml
  format: yaml
  label: Weights and Biases Service API
  slug: wandb-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-service-api-openapi.yml
- filename: wandb-table-api-openapi.yml
  format: yaml
  label: Weights and Biases Table API
  slug: wandb-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-table-api-openapi.yml
- filename: wandb-tables-api-openapi.yml
  format: yaml
  label: Weights and Biases Tables API
  slug: wandb-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/openapi/wandb-tables-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wandb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weights and Biases secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weights and Biases
provider_slug: wandb
scheme_count: 1
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/wandb-openapi.json
  type: http
slug: wandb-authentication
source_filename: wandb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wandb-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/wandb-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wandb/refs/heads/main/authentication/wandb-authentication.yml
summary_line: http · 1 scheme
tags:
- MLOps
- Experiment Tracking
- LLM Observability
- Model Registry
- AI Platform
- Evaluation
- Tracing
---
