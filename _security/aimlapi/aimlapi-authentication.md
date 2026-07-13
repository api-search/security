---
api_key_in: []
api_specs:
- filename: aimlapi-openapi.yml
  format: yaml
  label: AIMLAPI
  slug: aimlapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aimlapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIMLAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIMLAPI
provider_slug: aimlapi
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aimlapi-openapi.yml
  type: http
slug: aimlapi-authentication
source_filename: aimlapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aimlapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aimlapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/authentication/aimlapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- AI Models
- LLM
- Image Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
---
