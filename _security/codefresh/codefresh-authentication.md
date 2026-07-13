---
api_key_in:
- header
api_specs:
- filename: codefresh-openapi.yml
  format: yaml
  label: Codefresh REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codefresh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codefresh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codefresh
provider_slug: codefresh
scheme_count: 1
schemes:
- description: Codefresh API key. Send raw token as Authorization header value.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/codefresh-openapi.yml
  type: apiKey
slug: codefresh-authentication
source_filename: codefresh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codefresh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Codefresh API key. Send raw token as Authorization header value.\n  sources:\n  - openapi/codefresh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/authentication/codefresh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CI/CD
- Continuous Delivery
- GitOps
- Argo
- Kubernetes
- DevOps
- Pipelines
---
