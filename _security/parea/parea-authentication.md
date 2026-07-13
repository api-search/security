---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Parea REST API
  slug: parea-rest-api
  spec_type: OpenAPI
  url: https://docs.parea.ai/api-reference/overview
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Parea Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Parea AI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Parea AI
provider_slug: parea
scheme_count: 2
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/parea-rest-api-openapi.yml
  type: oauth2
- in: header
  name: APIKeyHeader
  parameter: x-api-key
  sources:
  - openapi/parea-rest-api-openapi.yml
  type: apiKey
slug: parea-authentication
source_filename: parea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parea-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/parea-rest-api-openapi.yml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/parea-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parea/refs/heads/main/authentication/parea-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- LLM
- Evaluation
- Observability
- Testing
- Prompt Management
- AI Engineering
- Machine Learning
- Tracing
- Experimentation
- Human Feedback
---
