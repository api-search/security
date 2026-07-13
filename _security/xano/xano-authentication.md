---
api_key_in: []
api_specs:
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Tables & Schema API
  slug: xano-metadata-tables-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Records & Content API
  slug: xano-metadata-records-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Files API
  slug: xano-metadata-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Branches & Workspace API
  slug: xano-metadata-branches-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata API Groups & Endpoints API
  slug: xano-metadata-api-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Auth & Access API
  slug: xano-metadata-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xano secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xano
provider_slug: xano
scheme_count: 1
schemes:
- description: 'Scoped Metadata API access token generated from your Xano instance settings (Instances > Metadata API > Manage Access Tokens). Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xano-openapi.yml
  type: http
slug: xano-authentication
source_filename: xano-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xano-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Scoped Metadata API access token generated from your Xano instance settings\n    (Instances > Metadata API > Manage Access Tokens). Sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/xano-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/authentication/xano-authentication.yml
summary_line: http · 1 scheme
tags:
- No Code
- Backend as a Service
- BaaS
- API Builder
- Database
- Serverless
---
