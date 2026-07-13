---
api_key_in: []
api_specs:
- filename: zenml-openapi.yml
  format: yaml
  label: ZenML OSS REST API
  slug: zenml-oss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zenml Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenML secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZenML
provider_slug: zenml
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zenml-openapi.yml
  type: http
slug: zenml-authentication
source_filename: zenml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zenml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/authentication/zenml-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Machine Learning
- MLOps
- LLMOps
- Pipelines
- Open Source
- Python
---
