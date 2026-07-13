---
api_key_in:
- header
api_specs:
- filename: weaviate-openapi.yml
  format: yaml
  label: Weaviate REST API
  slug: weaviate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weaviate/refs/heads/main/openapi/weaviate-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Weaviate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weaviate secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Weaviate
provider_slug: weaviate
scheme_count: 2
schemes:
- description: API key authentication
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/weaviate-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OIDC/JWT bearer authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/weaviate-openapi.yml
  type: http
slug: weaviate-authentication
source_filename: weaviate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weaviate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication\n  sources:\n  - openapi/weaviate-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OIDC/JWT bearer authentication\n  sources:\n  - openapi/weaviate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weaviate/refs/heads/main/authentication/weaviate-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Vector Database
- AI
- Machine Learning
- Semantic Search
- Open Source
- GraphQL
- Kubernetes
---
