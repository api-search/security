---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coreweave Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreWeave secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoreWeave
provider_slug: coreweave
scheme_count: 1
schemes:
- bearerFormat: API Access Token
  description: 'Provide a CoreWeave API access token using the `Authorization: Bearer

    {API_ACCESS_TOKEN}` header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/coreweave-openapi.yml
  type: http
slug: coreweave-authentication
source_filename: coreweave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coreweave-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Access Token\n  description: |-\n    Provide a CoreWeave API access token using the `Authorization: Bearer\n    {API_ACCESS_TOKEN}` header.\n  sources:\n  - openapi/coreweave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreweave/refs/heads/main/authentication/coreweave-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Cloud
- GPU
- HPC
- Inference
- Kubernetes
- Machine Learning
- Storage
---
