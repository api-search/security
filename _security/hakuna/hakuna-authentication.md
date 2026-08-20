---
api_key_in:
- header
api_specs:
- filename: hakuna-absences-api-openapi.yml
  format: yaml
  label: Hakuna Absences API
  slug: hakuna-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-absences-api-openapi.yml
- filename: hakuna-company-api-openapi.yml
  format: yaml
  label: Hakuna Company API
  slug: hakuna-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-company-api-openapi.yml
- filename: hakuna-management-api-openapi.yml
  format: yaml
  label: Hakuna Management API
  slug: hakuna-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-management-api-openapi.yml
- filename: hakuna-organization-api-openapi.yml
  format: yaml
  label: Hakuna Organization API
  slug: hakuna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-organization-api-openapi.yml
- filename: hakuna-overview-api-openapi.yml
  format: yaml
  label: Hakuna Overview API
  slug: hakuna-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-overview-api-openapi.yml
- filename: hakuna-projects-api-openapi.yml
  format: yaml
  label: Hakuna Projects API
  slug: hakuna-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-projects-api-openapi.yml
- filename: hakuna-tasks-api-openapi.yml
  format: yaml
  label: Hakuna Tasks API
  slug: hakuna-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-tasks-api-openapi.yml
- filename: hakuna-time-entries-api-openapi.yml
  format: yaml
  label: Hakuna Time Entries API
  slug: hakuna-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-time-entries-api-openapi.yml
- filename: hakuna-timer-api-openapi.yml
  format: yaml
  label: Hakuna Timer API
  slug: hakuna-timer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-timer-api-openapi.yml
- filename: hakuna-users-api-openapi.yml
  format: yaml
  label: Hakuna Users API
  slug: hakuna-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hakuna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hakuna secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hakuna
provider_slug: hakuna
scheme_count: 1
schemes:
- description: Personal API token managed under "My Settings". Organization endpoints require a separate organization-level token; management endpoints require an admin token.
  in: header
  name: AuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/hakuna-openapi.yml
  type: apiKey
slug: hakuna-authentication
source_filename: hakuna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hakuna-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Personal API token managed under \"My Settings\". Organization endpoints require\n    a separate organization-level token; management endpoints require an admin token.\n  sources:\n  - openapi/hakuna-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/authentication/hakuna-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Time Tracking
- HR
- Workforce Management
- Absence Management
- Project Tracking
- Software-as-a-Service
- Switzerland
- SME
---
