---
api_key_in:
- header
api_specs:
- filename: automation-anywhere-control-room-openapi.yml
  format: yaml
  label: Automation Anywhere Control Room API
  slug: control-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-control-room-openapi.yml
- filename: automation-anywhere-bot-deploy-openapi.yml
  format: yaml
  label: Automation Anywhere Bot Deploy API
  slug: bot-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-bot-deploy-openapi.yml
- filename: automation-anywhere-workload-management-openapi.yml
  format: yaml
  label: Automation Anywhere Workload Management API
  slug: workload-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-workload-management-openapi.yml
- filename: automation-anywhere-bot-insight-openapi.yml
  format: yaml
  label: Automation Anywhere Bot Insight API
  slug: bot-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-bot-insight-openapi.yml
- filename: automation-anywhere-api-task-execution-openapi.yml
  format: yaml
  label: Automation Anywhere API Task Execution API
  slug: api-task-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-api-task-execution-openapi.yml
- filename: automation-anywhere-credential-vault-openapi.yml
  format: yaml
  label: Automation Anywhere Credential Vault API
  slug: credential-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-credential-vault-openapi.yml
- filename: automation-anywhere-repository-management-openapi.yml
  format: yaml
  label: Automation Anywhere Repository Management API
  slug: repository-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-repository-management-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Automation Anywhere Authentication
name_suffix: Authentication
oauth_flows: []
overview: automation-anywhere secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: automation-anywhere
provider_slug: automation-anywhere
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the Authentication API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/automation-anywhere-api-task-execution-openapi.yml
  - openapi/automation-anywhere-bot-deploy-openapi.yml
  - openapi/automation-anywhere-bot-insight-openapi.yml
  - openapi/automation-anywhere-control-room-openapi.yml
  - openapi/automation-anywhere-credential-vault-openapi.yml
  - openapi/automation-anywhere-repository-management-openapi.yml
  - openapi/automation-anywhere-workload-management-openapi.yml
  type: http
- description: JWT token obtained from the Authentication API
  in: header
  name: xAuthorization
  parameter: X-Authorization
  sources:
  - openapi/automation-anywhere-api-task-execution-openapi.yml
  - openapi/automation-anywhere-bot-deploy-openapi.yml
  - openapi/automation-anywhere-bot-insight-openapi.yml
  - openapi/automation-anywhere-control-room-openapi.yml
  - openapi/automation-anywhere-credential-vault-openapi.yml
  - openapi/automation-anywhere-repository-management-openapi.yml
  - openapi/automation-anywhere-workload-management-openapi.yml
  type: apiKey
slug: automation-anywhere-authentication
source_filename: automation-anywhere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/automation-anywhere-api-task-execution-openapi.yml, openapi/automation-anywhere-bot-deploy-openapi.yml,\n  openapi/automation-anywhere-bot-insight-openapi.yml, openapi/automation-anywhere-control-room-openapi.yml,\n  openapi/automation-anywhere-credential-vault-openapi.yml, openapi/automation-anywhere-repository-management-openapi.yml,\n  openapi/automation-anywhere-workload-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the Authentication API\n  sources:\n  - openapi/automation-anywhere-api-task-execution-openapi.yml\n  - openapi/automation-anywhere-bot-deploy-openapi.yml\n  - openapi/automation-anywhere-bot-insight-openapi.yml\n  - openapi/automation-anywhere-control-room-openapi.yml\n  - openapi/automation-anywhere-credential-vault-openapi.yml\n  -\
  \ openapi/automation-anywhere-repository-management-openapi.yml\n  - openapi/automation-anywhere-workload-management-openapi.yml\n- name: xAuthorization\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  description: JWT token obtained from the Authentication API\n  sources:\n  - openapi/automation-anywhere-api-task-execution-openapi.yml\n  - openapi/automation-anywhere-bot-deploy-openapi.yml\n  - openapi/automation-anywhere-bot-insight-openapi.yml\n  - openapi/automation-anywhere-control-room-openapi.yml\n  - openapi/automation-anywhere-credential-vault-openapi.yml\n  - openapi/automation-anywhere-repository-management-openapi.yml\n  - openapi/automation-anywhere-workload-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/authentication/automation-anywhere-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
