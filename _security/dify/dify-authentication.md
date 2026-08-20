---
api_key_in: []
api_specs:
- filename: dify-chat-api-openapi.yml
  format: yaml
  label: Dify Chat API
  slug: dify-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-chat-api-openapi.yml
- filename: dify-completion-api-openapi.yml
  format: yaml
  label: Dify Completion API
  slug: dify-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-completion-api-openapi.yml
- filename: dify-conversations-api-openapi.yml
  format: yaml
  label: Dify Conversations API
  slug: dify-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-conversations-api-openapi.yml
- filename: dify-datasets-api-openapi.yml
  format: yaml
  label: Dify Datasets API
  slug: dify-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-datasets-api-openapi.yml
- filename: dify-files-api-openapi.yml
  format: yaml
  label: Dify Files API
  slug: dify-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-files-api-openapi.yml
- filename: dify-workflows-api-openapi.yml
  format: yaml
  label: Dify Workflows API
  slug: dify-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dify
provider_slug: dify
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dify-openapi.yml
  type: http
slug: dify-authentication
source_filename: dify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/authentication/dify-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Backend-as-a-Service
- LLMOps
---
