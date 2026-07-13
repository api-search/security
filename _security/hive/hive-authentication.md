---
api_key_in:
- header
api_specs:
- filename: hive-openapi.yml
  format: yaml
  label: Hive Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hive
provider_slug: hive
scheme_count: 1
schemes:
- description: Workspace-scoped API token issued from Hive admin settings.
  in: header
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/hive-openapi.yml
  type: apiKey
slug: hive-authentication
source_filename: hive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hive-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Workspace-scoped API token issued from Hive admin settings.\n  sources:\n  - openapi/hive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/authentication/hive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Task Management
- Team Collaboration
- Productivity
- Workflow Automation
- Time Tracking
---
