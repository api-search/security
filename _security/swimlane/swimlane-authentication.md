---
api_key_in:
- header
api_specs:
- filename: swimlane-applications-api-openapi.yml
  format: yaml
  label: Swimlane Applications API
  slug: swimlane-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-applications-api-openapi.yml
- filename: swimlane-authentication-api-openapi.yml
  format: yaml
  label: Swimlane Authentication API
  slug: swimlane-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-authentication-api-openapi.yml
- filename: swimlane-groups-api-openapi.yml
  format: yaml
  label: Swimlane Groups API
  slug: swimlane-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-groups-api-openapi.yml
- filename: swimlane-logging-api-openapi.yml
  format: yaml
  label: Swimlane Logging API
  slug: swimlane-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-logging-api-openapi.yml
- filename: swimlane-records-api-openapi.yml
  format: yaml
  label: Swimlane Records API
  slug: swimlane-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-records-api-openapi.yml
- filename: swimlane-reports-api-openapi.yml
  format: yaml
  label: Swimlane Reports API
  slug: swimlane-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-reports-api-openapi.yml
- filename: swimlane-settings-api-openapi.yml
  format: yaml
  label: Swimlane Settings API
  slug: swimlane-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-settings-api-openapi.yml
- filename: swimlane-tasks-api-openapi.yml
  format: yaml
  label: Swimlane Tasks API
  slug: swimlane-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-tasks-api-openapi.yml
- filename: swimlane-users-api-openapi.yml
  format: yaml
  label: Swimlane Users API
  slug: swimlane-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Swimlane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swimlane secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swimlane
provider_slug: swimlane
scheme_count: 2
schemes:
- description: JWT bearer token obtained from the user/login endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/swimlane-rest-api-openapi.yml
  type: http
- description: Personal Access Token (PAT) generated within the Swimlane platform
  in: header
  name: PrivateTokenAuth
  parameter: Private-Token
  sources:
  - openapi/swimlane-rest-api-openapi.yml
  type: apiKey
slug: swimlane-authentication
source_filename: swimlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swimlane-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: JWT bearer token obtained from the user/login endpoint\n  sources:\n  - openapi/swimlane-rest-api-openapi.yml\n- name: PrivateTokenAuth\n  type: apiKey\n  in: header\n  parameter: Private-Token\n  description: Personal Access Token (PAT) generated within the Swimlane platform\n  sources:\n  - openapi/swimlane-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/authentication/swimlane-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- SOAR
- Security Orchestration
- Automation
- Incident Response
- Playbooks
- Case Management
- Security Operations
- Agentic AI
---
