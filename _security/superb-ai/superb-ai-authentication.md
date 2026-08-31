---
api_key_in: []
api_specs:
- filename: superb-ai-mlops-platform-openapi.json
  format: json
  label: Superb AI MLOps Platform API
  slug: superb-ai-mlops-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/openapi/superb-ai-mlops-platform-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Superb Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superb AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Superb AI
provider_slug: superb-ai
scheme_count: 1
schemes:
- description: Cognito access token
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/superb-ai-mlops-platform-openapi.json
  type: http
slug: superb-ai-authentication
source_filename: superb-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/superb-ai-mlops-platform-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: Cognito access token\n  sources:\n  - openapi/superb-ai-mlops-platform-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/authentication/superb-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Data Labeling
- Annotation
- MLOps
- Training Data
- Model Training
- Inference
- Datasets
---
