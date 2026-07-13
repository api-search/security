---
api_key_in:
- header
api_specs:
- filename: publer-openapi.yml
  format: yaml
  label: Publer Posts & Scheduling API
  slug: posts-scheduling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Workspaces API
  slug: workspaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Publer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Publer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Publer
provider_slug: publer
scheme_count: 2
schemes:
- description: 'API key passed as `Authorization: Bearer-API YOUR_API_KEY`. A `Publer-Workspace-Id` header is also required to scope requests to a workspace.'
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/publer-openapi.yml
  type: apiKey
- description: The id of the workspace to scope the request to.
  in: header
  name: workspace_id
  parameter: Publer-Workspace-Id
  sources:
  - openapi/publer-openapi.yml
  type: apiKey
slug: publer-authentication
source_filename: publer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/publer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key passed as `Authorization: Bearer-API YOUR_API_KEY`. A `Publer-Workspace-Id`\n    header is also required to scope requests to a workspace.'\n  sources:\n  - openapi/publer-openapi.yml\n- name: workspace_id\n  type: apiKey\n  in: header\n  parameter: Publer-Workspace-Id\n  description: The id of the workspace to scope the request to.\n  sources:\n  - openapi/publer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/authentication/publer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Social Media
- Scheduling
- Publishing
- Content Management
- Marketing
---
