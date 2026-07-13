---
api_key_in: []
api_specs:
- filename: argo-workflows-openapi.yml
  format: yaml
  label: Argo Workflows API
  slug: argo-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-workflows-openapi.yml
- filename: argo-cd-openapi.yml
  format: yaml
  label: Argo CD API
  slug: argo-cd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-cd-openapi.yml
- filename: argo-events-asyncapi.yml
  format: yaml
  label: Argo Events API
  slug: argo-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/asyncapi/argo-events-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Argo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo
provider_slug: argo
scheme_count: 1
schemes:
- description: Bearer token obtained from the POST /session endpoint using username/password or from an external OIDC provider configured in Argo CD.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/argo-cd-openapi.yml
  - openapi/argo-workflows-openapi.yml
  type: http
slug: argo-authentication
source_filename: argo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-cd-openapi.yml, openapi/argo-workflows-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the POST /session endpoint using username/password\n    or from an external OIDC provider configured in Argo CD.\n  sources:\n  - openapi/argo-cd-openapi.yml\n  - openapi/argo-workflows-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/authentication/argo-authentication.yml
summary_line: http · 1 scheme
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
---
