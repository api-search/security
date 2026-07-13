---
api_key_in: []
api_specs:
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Instances API
  slug: instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Databases API
  slug: databases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Issues / Migrations API
  slug: issues-migrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Rollouts API
  slug: rollouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Sheets API
  slug: sheets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Users / Roles API
  slug: users-roles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bytebase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bytebase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bytebase
provider_slug: bytebase
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Access token obtained from POST /v1/auth/login using a service-account email and service key. Supplied as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bytebase-openapi.yml
  type: http
slug: bytebase-authentication
source_filename: bytebase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bytebase-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token obtained from POST /v1/auth/login using a service-account email\n    and service key. Supplied as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/bytebase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/authentication/bytebase-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- DevOps
- Schema Migration
- CI/CD
- DevSecOps
---
