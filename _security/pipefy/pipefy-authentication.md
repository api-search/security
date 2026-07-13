---
api_key_in: []
api_specs:
- filename: pipefy-openapi.yml
  format: yaml
  label: Pipefy GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipefy/refs/heads/main/openapi/pipefy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pipefy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pipefy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pipefy
provider_slug: pipefy
scheme_count: 1
schemes:
- description: 'Personal Access Token or Service Account token. Pass as

    `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pipefy-openapi.yml
  type: http
slug: pipefy-authentication
source_filename: pipefy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pipefy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Personal Access Token or Service Account token. Pass as\n    `Authorization: Bearer <token>`.\n  sources:\n  - openapi/pipefy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipefy/refs/heads/main/authentication/pipefy-authentication.yml
summary_line: http · 1 scheme
tags:
- Workflow Automation
- Business Process Management
- No-Code
- BPM
- GraphQL
- Process Orchestration
---
