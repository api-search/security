---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Weights And Biases Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weights & Biases secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weights & Biases
provider_slug: weights-and-biases
scheme_count: 1
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/weights-and-biases-openapi.json
  type: http
slug: weights-and-biases-authentication
source_filename: weights-and-biases-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weights-and-biases-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/weights-and-biases-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/authentication/weights-and-biases-authentication.yml
summary_line: http · 1 scheme
tags:
- ML
- MLOps
- Experiment Tracking
- Model Registry
- GenAI
---
