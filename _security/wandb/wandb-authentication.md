---
api_key_in: []
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
