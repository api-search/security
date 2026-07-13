---
api_key_in: []
api_specs:
- filename: preset-openapi.yml
  format: yaml
  label: Preset Auth API
  slug: preset-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Teams and Workspaces API
  slug: preset-teams-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Dashboards API
  slug: preset-superset-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Charts API
  slug: preset-superset-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Datasets API
  slug: preset-superset-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Databases API
  slug: preset-superset-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset SQL Lab API
  slug: preset-superset-sqllab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
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
