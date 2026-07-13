---
api_key_in:
- header
api_specs:
- filename: argo-workflows-openapi.json
  format: json
  label: Argo Workflows API
  slug: argo-workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Argo Workflows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo Workflows secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo Workflows
provider_slug: argo-workflows
scheme_count: 1
schemes:
- description: JWT Bearer token
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/argo-workflows-openapi.json
  type: apiKey
slug: argo-workflows-authentication
source_filename: argo-workflows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-workflows-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT Bearer token\n  sources:\n  - openapi/argo-workflows-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/authentication/argo-workflows-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
---
