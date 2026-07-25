---
api_key_in: []
api_specs:
- filename: acronis-activities-api-openapi.yml
  format: yaml
  label: Acronis Activities API
  slug: acronis-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-activities-api-openapi.yml
- filename: acronis-agent-updates-api-openapi.yml
  format: yaml
  label: Acronis Agent Updates API
  slug: acronis-agent-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agent-updates-api-openapi.yml
- filename: acronis-agents-api-openapi.yml
  format: yaml
  label: Acronis Agents API
  slug: acronis-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agents-api-openapi.yml
- filename: acronis-authentication-api-openapi.yml
  format: yaml
  label: Acronis Authentication API
  slug: acronis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-authentication-api-openapi.yml
- filename: acronis-clients-api-openapi.yml
  format: yaml
  label: Acronis Clients API
  slug: acronis-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-clients-api-openapi.yml
- filename: acronis-hardware-nodes-api-openapi.yml
  format: yaml
  label: Acronis Hardware Nodes API
  slug: acronis-hardware-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-hardware-nodes-api-openapi.yml
- filename: acronis-licensing-api-openapi.yml
  format: yaml
  label: Acronis Licensing API
  slug: acronis-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-licensing-api-openapi.yml
- filename: acronis-tasks-api-openapi.yml
  format: yaml
  label: Acronis Tasks API
  slug: acronis-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-tasks-api-openapi.yml
- filename: acronis-tenants-api-openapi.yml
  format: yaml
  label: Acronis Tenants API
  slug: acronis-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-tenants-api-openapi.yml
- filename: acronis-usage-api-openapi.yml
  format: yaml
  label: Acronis Usage API
  slug: acronis-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-usage-api-openapi.yml
- filename: acronis-users-api-openapi.yml
  format: yaml
  label: Acronis Users API
  slug: acronis-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-users-api-openapi.yml
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
