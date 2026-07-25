---
api_key_in: []
api_specs:
- filename: preset-authentication-api-openapi.yml
  format: yaml
  label: Preset Authentication API
  slug: preset-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-authentication-api-openapi.yml
- filename: preset-charts-api-openapi.yml
  format: yaml
  label: Preset Charts API
  slug: preset-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-charts-api-openapi.yml
- filename: preset-dashboards-api-openapi.yml
  format: yaml
  label: Preset Dashboards API
  slug: preset-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-dashboards-api-openapi.yml
- filename: preset-databases-api-openapi.yml
  format: yaml
  label: Preset Databases API
  slug: preset-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-databases-api-openapi.yml
- filename: preset-datasets-api-openapi.yml
  format: yaml
  label: Preset Datasets API
  slug: preset-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-datasets-api-openapi.yml
- filename: preset-sql-lab-api-openapi.yml
  format: yaml
  label: Preset SQL Lab API
  slug: preset-sql-lab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-sql-lab-api-openapi.yml
- filename: preset-teams-api-openapi.yml
  format: yaml
  label: Preset Teams API
  slug: preset-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-teams-api-openapi.yml
- filename: preset-workspaces-api-openapi.yml
  format: yaml
  label: Preset Workspaces API
  slug: preset-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Preset Authentication
name_suffix: Authentication
oauth_flows: []
overview: Preset secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Preset
provider_slug: preset
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT obtained from POST /v1/auth/ by exchanging an API token name and secret. Passed as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/preset-openapi.yml
  type: http
slug: preset-authentication
source_filename: preset-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/preset-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT obtained from POST /v1/auth/ by exchanging an API token name and secret.\n    Passed as Authorization: Bearer <token>.'\n  sources:\n  - openapi/preset-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/authentication/preset-authentication.yml
summary_line: http · 1 scheme
tags:
- BI
- Analytics
- Superset
- Dashboards
- Data Visualization
---
