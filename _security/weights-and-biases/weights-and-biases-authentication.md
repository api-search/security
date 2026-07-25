---
api_key_in: []
api_specs:
- filename: weights-and-biases-calls-api-openapi.yml
  format: yaml
  label: Weights & Biases Calls API
  slug: weights-and-biases-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-calls-api-openapi.yml
- filename: weights-and-biases-costs-api-openapi.yml
  format: yaml
  label: Weights & Biases Costs API
  slug: weights-and-biases-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-costs-api-openapi.yml
- filename: weights-and-biases-feedback-api-openapi.yml
  format: yaml
  label: Weights & Biases Feedback API
  slug: weights-and-biases-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-feedback-api-openapi.yml
- filename: weights-and-biases-files-api-openapi.yml
  format: yaml
  label: Weights & Biases Files API
  slug: weights-and-biases-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-files-api-openapi.yml
- filename: weights-and-biases-objects-api-openapi.yml
  format: yaml
  label: Weights & Biases Objects API
  slug: weights-and-biases-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-objects-api-openapi.yml
- filename: weights-and-biases-refs-api-openapi.yml
  format: yaml
  label: Weights & Biases Refs API
  slug: weights-and-biases-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-refs-api-openapi.yml
- filename: weights-and-biases-service-api-openapi.yml
  format: yaml
  label: Weights & Biases Service API
  slug: weights-and-biases-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-service-api-openapi.yml
- filename: weights-and-biases-table-api-openapi.yml
  format: yaml
  label: Weights & Biases Table API
  slug: weights-and-biases-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-table-api-openapi.yml
- filename: weights-and-biases-tables-api-openapi.yml
  format: yaml
  label: Weights & Biases Tables API
  slug: weights-and-biases-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/openapi/weights-and-biases-tables-api-openapi.yml
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
