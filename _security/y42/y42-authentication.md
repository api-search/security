---
api_key_in: []
api_specs:
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Spaces API
  slug: y42-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Orchestration API
  slug: y42-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Runs API
  slug: y42-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Manifest API
  slug: y42-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Y42 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Y42 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Y42
provider_slug: y42
scheme_count: 1
schemes:
- description: Y42 API keys are created in the organization settings inside the Y42 app and passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/y42-openapi.yml
  type: http
slug: y42-authentication
source_filename: y42-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/y42-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Y42 API keys are created in the organization settings inside the Y42 app and\n    passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/y42-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/authentication/y42-authentication.yml
summary_line: http · 1 scheme
tags:
- DataOps
- Data Pipelines
- Orchestration
- dbt
- Snowflake
- BigQuery
- GitOps
---
