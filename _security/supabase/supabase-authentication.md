---
api_key_in:
- header
api_specs:
- filename: supabase-management-api-openapi.yml
  format: yaml
  label: Supabase Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-management-api-openapi.yml
- filename: supabase-auth-api-openapi.yml
  format: yaml
  label: Supabase Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-auth-api-openapi.yml
- filename: supabase-storage-api-openapi.yml
  format: yaml
  label: Supabase Storage API
  slug: storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-storage-api-openapi.yml
- filename: supabase-database-rest-api-openapi.yml
  format: yaml
  label: Supabase Database REST API
  slug: database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-database-rest-api-openapi.yml
- filename: supabase-edge-functions-api-openapi.yml
  format: yaml
  label: Supabase Edge Functions API
  slug: edge-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-edge-functions-api-openapi.yml
- filename: supabase-realtime-api-asyncapi.yml
  format: yaml
  label: Supabase Realtime API
  slug: realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/asyncapi/supabase-realtime-api-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Supabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supabase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Supabase
provider_slug: supabase
scheme_count: 2
schemes:
- description: Supabase project API key (anon key for public operations, service_role key for admin operations).
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/supabase-auth-api-openapi.yml
  - openapi/supabase-database-rest-api-openapi.yml
  - openapi/supabase-edge-functions-api-openapi.yml
  - openapi/supabase-storage-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT access token obtained from a successful authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/supabase-auth-api-openapi.yml
  - openapi/supabase-database-rest-api-openapi.yml
  - openapi/supabase-edge-functions-api-openapi.yml
  - openapi/supabase-management-api-openapi.yml
  - openapi/supabase-storage-api-openapi.yml
  type: http
slug: supabase-authentication
source_filename: supabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/supabase-auth-api-openapi.yml, openapi/supabase-database-rest-api-openapi.yml,\n  openapi/supabase-edge-functions-api-openapi.yml, openapi/supabase-management-api-openapi.yml,\n  openapi/supabase-storage-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Supabase project API key (anon key for public operations, service_role key for\n    admin operations).\n  sources:\n  - openapi/supabase-auth-api-openapi.yml\n  - openapi/supabase-database-rest-api-openapi.yml\n  - openapi/supabase-edge-functions-api-openapi.yml\n  - openapi/supabase-storage-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token obtained from a successful authentication.\n  sources:\n  - openapi/supabase-auth-api-openapi.yml\n  - openapi/supabase-database-rest-api-openapi.yml\n\
  \  - openapi/supabase-edge-functions-api-openapi.yml\n  - openapi/supabase-management-api-openapi.yml\n  - openapi/supabase-storage-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/authentication/supabase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Backend As A Service
- PostgreSQL
- Open Source
- Authentication
- Real Time
- Storage
- Edge Functions
- Database
---
