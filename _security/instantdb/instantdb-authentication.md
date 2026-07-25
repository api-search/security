---
api_key_in: []
api_specs:
- filename: instantdb-asyncapi.yml
  format: yaml
  label: InstantDB Realtime Sync API
  slug: instantdb-realtime-sync-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/asyncapi/instantdb-asyncapi.yml
- filename: instantdb-auth-api-openapi.yml
  format: yaml
  label: InstantDB Auth API
  slug: instantdb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-auth-api-openapi.yml
- filename: instantdb-presence-api-openapi.yml
  format: yaml
  label: InstantDB Presence API
  slug: instantdb-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-presence-api-openapi.yml
- filename: instantdb-query-api-openapi.yml
  format: yaml
  label: InstantDB Query API
  slug: instantdb-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-query-api-openapi.yml
- filename: instantdb-storage-api-openapi.yml
  format: yaml
  label: InstantDB Storage API
  slug: instantdb-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-storage-api-openapi.yml
- filename: instantdb-transactions-api-openapi.yml
  format: yaml
  label: InstantDB Transactions API
  slug: instantdb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Instantdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: InstantDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InstantDB
provider_slug: instantdb
scheme_count: 1
schemes:
- description: 'Admin token issued in the InstantDB dashboard, sent as `Authorization: Bearer $ADMIN_TOKEN`.'
  name: adminToken
  scheme: bearer
  sources:
  - openapi/instantdb-openapi.yml
  type: http
slug: instantdb-authentication
source_filename: instantdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instantdb-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: adminToken\n  type: http\n  scheme: bearer\n  description: 'Admin token issued in the InstantDB dashboard, sent as `Authorization: Bearer\n    $ADMIN_TOKEN`.'\n  sources:\n  - openapi/instantdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/authentication/instantdb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Realtime
- Sync
- Backend
- Local First
---
