---
api_key_in:
- header
api_specs:
- filename: askui-workspace-service-openapi-original.json
  format: json
  label: AskUI Workspaces API
  slug: askui-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askui/refs/heads/main/openapi/askui-workspace-service-openapi-original.json
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
