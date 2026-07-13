---
api_key_in: []
api_specs:
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Inference Endpoints API
  slug: inferless-inference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Model Management API
  slug: inferless-model-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Workspaces and Deployments
  slug: inferless-workspaces-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inferless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inferless secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inferless
provider_slug: inferless
scheme_count: 1
schemes:
- description: Workspace API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/inferless-openapi.yml
  type: http
slug: inferless-authentication
source_filename: inferless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inferless-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Workspace API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/inferless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/authentication/inferless-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- ML Inference
- Serverless GPU
- Model Deployment
- Inference
---
