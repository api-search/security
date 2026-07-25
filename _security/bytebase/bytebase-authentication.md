---
api_key_in: []
api_specs:
- filename: bytebase-auth-api-openapi.yml
  format: yaml
  label: Bytebase Auth API
  slug: bytebase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-auth-api-openapi.yml
- filename: bytebase-databases-api-openapi.yml
  format: yaml
  label: Bytebase Databases API
  slug: bytebase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-databases-api-openapi.yml
- filename: bytebase-groups-api-openapi.yml
  format: yaml
  label: Bytebase Groups API
  slug: bytebase-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-groups-api-openapi.yml
- filename: bytebase-instances-api-openapi.yml
  format: yaml
  label: Bytebase Instances API
  slug: bytebase-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-instances-api-openapi.yml
- filename: bytebase-issues-api-openapi.yml
  format: yaml
  label: Bytebase Issues API
  slug: bytebase-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-issues-api-openapi.yml
- filename: bytebase-plans-api-openapi.yml
  format: yaml
  label: Bytebase Plans API
  slug: bytebase-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-plans-api-openapi.yml
- filename: bytebase-projects-api-openapi.yml
  format: yaml
  label: Bytebase Projects API
  slug: bytebase-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-projects-api-openapi.yml
- filename: bytebase-roles-api-openapi.yml
  format: yaml
  label: Bytebase Roles API
  slug: bytebase-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-roles-api-openapi.yml
- filename: bytebase-rollouts-api-openapi.yml
  format: yaml
  label: Bytebase Rollouts API
  slug: bytebase-rollouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-rollouts-api-openapi.yml
- filename: bytebase-sheets-api-openapi.yml
  format: yaml
  label: Bytebase Sheets API
  slug: bytebase-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-sheets-api-openapi.yml
- filename: bytebase-users-api-openapi.yml
  format: yaml
  label: Bytebase Users API
  slug: bytebase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-users-api-openapi.yml
- filename: bytebase-webhooks-api-openapi.yml
  format: yaml
  label: Bytebase Webhooks API
  slug: bytebase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-webhooks-api-openapi.yml
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
