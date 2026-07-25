---
api_key_in: []
api_specs:
- filename: talend-connections-api-openapi.yml
  format: yaml
  label: Talend Cloud Connections API
  slug: talend-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-connections-api-openapi.yml
- filename: talend-artifacts-api-openapi.yml
  format: yaml
  label: Talend Artifacts API
  slug: talend-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-artifacts-api-openapi.yml
- filename: talend-connections-api-openapi.yml
  format: yaml
  label: Talend Connections API
  slug: talend-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-connections-api-openapi.yml
- filename: talend-environments-api-openapi.yml
  format: yaml
  label: Talend Environments API
  slug: talend-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-environments-api-openapi.yml
- filename: talend-plan-executions-api-openapi.yml
  format: yaml
  label: Talend Plan Executions API
  slug: talend-plan-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-plan-executions-api-openapi.yml
- filename: talend-plans-api-openapi.yml
  format: yaml
  label: Talend Plans API
  slug: talend-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-plans-api-openapi.yml
- filename: talend-promotion-executions-api-openapi.yml
  format: yaml
  label: Talend Promotion Executions API
  slug: talend-promotion-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-promotion-executions-api-openapi.yml
- filename: talend-promotions-api-openapi.yml
  format: yaml
  label: Talend Promotions API
  slug: talend-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-promotions-api-openapi.yml
- filename: talend-remote-engine-clusters-api-openapi.yml
  format: yaml
  label: Talend Remote Engine Clusters API
  slug: talend-remote-engine-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-remote-engine-clusters-api-openapi.yml
- filename: talend-remote-engines-api-openapi.yml
  format: yaml
  label: Talend Remote Engines API
  slug: talend-remote-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-remote-engines-api-openapi.yml
- filename: talend-run-profiles-api-openapi.yml
  format: yaml
  label: Talend Run Profiles API
  slug: talend-run-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-run-profiles-api-openapi.yml
- filename: talend-schedules-api-openapi.yml
  format: yaml
  label: Talend Schedules API
  slug: talend-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-schedules-api-openapi.yml
- filename: talend-task-executions-api-openapi.yml
  format: yaml
  label: Talend Task Executions API
  slug: talend-task-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-task-executions-api-openapi.yml
- filename: talend-tasks-api-openapi.yml
  format: yaml
  label: Talend Tasks API
  slug: talend-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-tasks-api-openapi.yml
- filename: talend-workspaces-api-openapi.yml
  format: yaml
  label: Talend Workspaces API
  slug: talend-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Talend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talend
provider_slug: talend
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token from Talend Cloud personal access token or service account token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/talend-orchestration-openapi.yml
  - openapi/talend-processing-openapi.yml
  type: http
slug: talend-authentication
source_filename: talend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talend-orchestration-openapi.yml, openapi/talend-processing-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token from Talend Cloud personal access token or service account token\n  sources:\n  - openapi/talend-orchestration-openapi.yml\n  - openapi/talend-processing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/authentication/talend-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Data Integration
- Data Quality
- ETL
- Orchestration
- Pipelines
---
