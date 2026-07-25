---
api_key_in:
- header
api_specs:
- filename: absentify-absences-api-openapi.yml
  format: yaml
  label: Absentify Absences API
  slug: absentify-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-absences-api-openapi.yml
- filename: absentify-departments-api-openapi.yml
  format: yaml
  label: Absentify Departments API
  slug: absentify-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-departments-api-openapi.yml
- filename: absentify-leave-types-api-openapi.yml
  format: yaml
  label: Absentify Leave types API
  slug: absentify-leave-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-leave-types-api-openapi.yml
- filename: absentify-members-api-openapi.yml
  format: yaml
  label: Absentify Members API
  slug: absentify-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-members-api-openapi.yml
- filename: absentify-public-holidays-api-openapi.yml
  format: yaml
  label: Absentify Public holidays API
  slug: absentify-public-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-public-holidays-api-openapi.yml
- filename: absentify-requests-api-openapi.yml
  format: yaml
  label: Absentify Requests API
  slug: absentify-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-requests-api-openapi.yml
- filename: absentify-workspace-api-openapi.yml
  format: yaml
  label: Absentify Workspace API
  slug: absentify-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Absentify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Absentify secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Absentify
provider_slug: absentify
scheme_count: 2
schemes:
- in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/absentify-openapi.yml
  type: apiKey
- description: API key from your absentify account settings. Requires Plus plan.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/absentify-openapi.yml
  type: apiKey
slug: absentify-authentication
source_filename: absentify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/absentify-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/absentify-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from your absentify account settings. Requires Plus plan.\n  sources:\n  - openapi/absentify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/authentication/absentify-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
---
