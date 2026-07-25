---
api_key_in:
- header
api_specs:
- filename: askui-access-tokens-api-openapi.yml
  format: yaml
  label: AskUI access-tokens API
  slug: askui-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-access-tokens-api-openapi.yml
- filename: askui-agent-executions-api-openapi.yml
  format: yaml
  label: AskUI agent-executions API
  slug: askui-agent-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-agent-executions-api-openapi.yml
- filename: askui-agents-api-openapi.yml
  format: yaml
  label: AskUI agents API
  slug: askui-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-agents-api-openapi.yml
- filename: askui-analytics-api-openapi.yml
  format: yaml
  label: AskUI analytics API
  slug: askui-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-analytics-api-openapi.yml
- filename: askui-auth-api-openapi.yml
  format: yaml
  label: AskUI auth API
  slug: askui-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-auth-api-openapi.yml
- filename: askui-billing-api-openapi.yml
  format: yaml
  label: AskUI billing API
  slug: askui-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-billing-api-openapi.yml
- filename: askui-dashboard-api-openapi.yml
  format: yaml
  label: AskUI dashboard API
  slug: askui-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-dashboard-api-openapi.yml
- filename: askui-files-api-openapi.yml
  format: yaml
  label: AskUI files API
  slug: askui-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-files-api-openapi.yml
- filename: askui-invites-api-openapi.yml
  format: yaml
  label: AskUI invites API
  slug: askui-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-invites-api-openapi.yml
- filename: askui-runner-jobs-api-openapi.yml
  format: yaml
  label: AskUI runner-jobs API
  slug: askui-runner-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-runner-jobs-api-openapi.yml
- filename: askui-runs-api-openapi.yml
  format: yaml
  label: AskUI runs API
  slug: askui-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-runs-api-openapi.yml
- filename: askui-schedules-api-openapi.yml
  format: yaml
  label: AskUI schedules API
  slug: askui-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-schedules-api-openapi.yml
- filename: askui-tools-api-openapi.yml
  format: yaml
  label: AskUI tools API
  slug: askui-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-tools-api-openapi.yml
- filename: askui-workspace-memberships-api-openapi.yml
  format: yaml
  label: AskUI workspace-memberships API
  slug: askui-workspace-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-workspace-memberships-api-openapi.yml
- filename: askui-workspaces-api-openapi.yml
  format: yaml
  label: AskUI workspaces API
  slug: askui-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Askui Authentication
name_suffix: Authentication
oauth_flows: []
overview: AskUI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AskUI
provider_slug: askui
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/askui-workspace-service-openapi-original.json
  type: http
- in: header
  name: Basic
  parameter: Authorization
  sources:
  - openapi/askui-workspace-service-openapi-original.json
  type: apiKey
slug: askui-authentication
source_filename: askui-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/askui-workspace-service-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/askui-workspace-service-openapi-original.json\n- name: Basic\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/askui-workspace-service-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/authentication/askui-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Test Automation
- UI Automation
- AI Agents
- Computer Use
- Vision Agent
- Quality Assurance
- Mobile Testing
- RPA
---
