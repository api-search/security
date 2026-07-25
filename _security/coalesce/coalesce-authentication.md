---
api_key_in: []
api_specs:
- filename: coalesce-environments-api-openapi.yml
  format: yaml
  label: Coalesce Environments API
  slug: coalesce-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-environments-api-openapi.yml
- filename: coalesce-git-accounts-api-openapi.yml
  format: yaml
  label: Coalesce Git Accounts API
  slug: coalesce-git-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-git-accounts-api-openapi.yml
- filename: coalesce-nodes-api-openapi.yml
  format: yaml
  label: Coalesce Nodes API
  slug: coalesce-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-nodes-api-openapi.yml
- filename: coalesce-projects-api-openapi.yml
  format: yaml
  label: Coalesce Projects API
  slug: coalesce-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-projects-api-openapi.yml
- filename: coalesce-runs-api-openapi.yml
  format: yaml
  label: Coalesce Runs API
  slug: coalesce-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-runs-api-openapi.yml
- filename: coalesce-scheduler-api-openapi.yml
  format: yaml
  label: Coalesce Scheduler API
  slug: coalesce-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-scheduler-api-openapi.yml
- filename: coalesce-users-api-openapi.yml
  format: yaml
  label: Coalesce Users API
  slug: coalesce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/coalesce-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coalesce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coalesce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coalesce
provider_slug: coalesce
scheme_count: 1
schemes:
- description: Bearer token obtained from the Deploy tab in the Coalesce application. Tokens never expire and remain valid across all environments and projects.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: coalesce-authentication
source_filename: coalesce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the Deploy tab in the Coalesce application. Tokens\n    never expire and remain valid across all environments and projects.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/authentication/coalesce-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Transformation
- Snowflake
- Data Pipelines
- Data Catalog
- Data Quality
- Analytics
- AI
---
