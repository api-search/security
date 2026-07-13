---
api_key_in: []
api_specs:
- filename: centml-openapi.yml
  format: yaml
  label: CentML Serverless Inference (Chat Completions) API
  slug: centml-serverless-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Models API
  slug: centml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Deployments / Endpoints API
  slug: centml-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Clusters API
  slug: centml-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Centml Authentication
name_suffix: Authentication
oauth_flows: []
overview: CentML secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CentML
provider_slug: centml
scheme_count: 1
schemes:
- bearerFormat: CentML API key
  description: 'Set the `Authorization: Bearer <CENTML_API_KEY>` header. Serverless inference uses a serverless token; the platform API uses an account access token. Both are issued from the CentML platform.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/centml-openapi.yml
  type: http
slug: centml-authentication
source_filename: centml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/centml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: CentML API key\n  description: 'Set the `Authorization: Bearer <CENTML_API_KEY>` header. Serverless inference\n    uses a serverless token; the platform API uses an account access token. Both are issued\n    from the CentML platform.'\n  sources:\n  - openapi/centml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/authentication/centml-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Serverless
- GPU
---
