---
api_key_in:
- header
api_specs:
- filename: argo-cd-openapi.json
  format: json
  label: Argo CD API
  slug: argo-cd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Argo Cd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo CD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo CD
provider_slug: argo-cd
scheme_count: 1
schemes:
- description: 'JWT Bearer token. Format: Bearer <token>'
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/argo-cd-openapi.json
  type: apiKey
slug: argo-cd-authentication
source_filename: argo-cd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-cd-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Bearer token. Format: Bearer <token>'\n  sources:\n  - openapi/argo-cd-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/authentication/argo-cd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
---
