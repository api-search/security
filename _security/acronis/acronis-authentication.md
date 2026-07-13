---
api_key_in: []
api_specs:
- filename: acronis-account-management-openapi.yaml
  format: yaml
  label: Acronis Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-account-management-openapi.yaml
- filename: acronis-agent-management-openapi.yaml
  format: yaml
  label: Acronis Agent Management REST API
  slug: agent-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agent-management-openapi.yaml
- filename: acronis-task-manager-openapi.yaml
  format: yaml
  label: Acronis Task Manager API
  slug: task-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-task-manager-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acronis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acronis secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Acronis
provider_slug: acronis
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth2 bearer token obtained from /idp/token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acronis-account-management-openapi.yaml
  - openapi/acronis-agent-management-openapi.yaml
  - openapi/acronis-task-manager-openapi.yaml
  type: http
- description: Base64-encoded client_id:client_secret
  name: basicAuth
  scheme: basic
  sources:
  - openapi/acronis-account-management-openapi.yaml
  type: http
slug: acronis-authentication
source_filename: acronis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acronis-account-management-openapi.yaml, openapi/acronis-agent-management-openapi.yaml,\n  openapi/acronis-task-manager-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 bearer token obtained from /idp/token\n  sources:\n  - openapi/acronis-account-management-openapi.yaml\n  - openapi/acronis-agent-management-openapi.yaml\n  - openapi/acronis-task-manager-openapi.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded client_id:client_secret\n  sources:\n  - openapi/acronis-account-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/authentication/acronis-authentication.yml
summary_line: http · 2 schemes
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
---
