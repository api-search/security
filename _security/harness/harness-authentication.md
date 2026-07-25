---
api_key_in:
- header
api_specs:
- filename: harness-organizations-api-openapi.yml
  format: yaml
  label: Harness Organizations API
  slug: harness-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-organizations-api-openapi.yml
- filename: harness-pipeline-execution-api-openapi.yml
  format: yaml
  label: Harness Pipeline Execution API
  slug: harness-pipeline-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-pipeline-execution-api-openapi.yml
- filename: harness-pipelines-api-openapi.yml
  format: yaml
  label: Harness Pipelines API
  slug: harness-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-pipelines-api-openapi.yml
- filename: harness-projects-api-openapi.yml
  format: yaml
  label: Harness Projects API
  slug: harness-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-projects-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harness Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harness secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harness
provider_slug: harness
scheme_count: 1
schemes:
- description: Harness API key.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/harness-platform-api.yaml
  type: apiKey
slug: harness-authentication
source_filename: harness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harness-platform-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Harness API key.\n  sources:\n  - openapi/harness-platform-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/authentication/harness-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- GitOps
- Internal Developer Portal
- Lifecycle
- Software Delivery
---
