---
api_key_in:
- header
api_specs:
- filename: nhost-authentication-openapi.yml
  format: yaml
  label: Nhost Authentication API
  slug: nhost-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-authentication-openapi.yml
- filename: nhost-storage-openapi.yml
  format: yaml
  label: Nhost Storage API
  slug: nhost-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-storage-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nhost secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nhost
provider_slug: nhost
scheme_count: 2
schemes:
- description: Bearer authentication with JWT access token. Used to authenticate requests to protected endpoints.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nhost-authentication-openapi.yml
  - openapi/nhost-storage-openapi.yml
  type: http
- description: Hasura admin secret key for backend/administrative operations.
  in: header
  name: X-Hasura-Admin-Secret
  parameter: X-Hasura-Admin-Secret
  sources:
  - openapi/nhost-storage-openapi.yml
  type: apiKey
slug: nhost-authentication
source_filename: nhost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nhost-authentication-openapi.yml, openapi/nhost-storage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication with JWT access token. Used to authenticate requests to\n    protected endpoints.\n  sources:\n  - openapi/nhost-authentication-openapi.yml\n  - openapi/nhost-storage-openapi.yml\n- name: X-Hasura-Admin-Secret\n  type: apiKey\n  in: header\n  parameter: X-Hasura-Admin-Secret\n  description: Hasura admin secret key for backend/administrative operations.\n  sources:\n  - openapi/nhost-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/authentication/nhost-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- GraphQL
- PostgreSQL
- Authentication
- File Storage
- Serverless Functions
- Real-Time
- Open Source
- Firebase Alternative
- Backend as a Service
- BaaS
---
