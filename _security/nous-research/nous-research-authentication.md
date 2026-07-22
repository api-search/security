---
api_key_in: []
api_specs:
- filename: nous-research-inference-api-openapi.yml
  format: yaml
  label: Nous Research Inference API (Nous Portal)
  slug: nous-research-inference-api-nous-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nous-research/refs/heads/main/openapi/nous-research-inference-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nous Research Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nous Research secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nous Research
provider_slug: nous-research
scheme_count: 1
schemes:
- description: 'Nous Portal API key supplied as: Authorization: Bearer <key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nous-research-inference-api-openapi.yml
  type: http
slug: nous-research-authentication
source_filename: nous-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nous-research-inference-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Nous Portal API key supplied as: Authorization: Bearer <key>'\n  sources:\n  - openapi/nous-research-inference-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nous-research/refs/heads/main/authentication/nous-research-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Machine Learning
- Large Language Models
- Inference
- Agents
- Open Weights
- x402
---
