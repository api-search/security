---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: thenile-auth-api-openapi.yml
  format: yaml
  label: Nile Auth API
  slug: thenile-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-auth-api-openapi.yml
- filename: thenile-authentication-api-openapi.yml
  format: yaml
  label: Nile Authentication API
  slug: thenile-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-authentication-api-openapi.yml
- filename: thenile-compute-api-openapi.yml
  format: yaml
  label: Nile Compute API
  slug: thenile-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-compute-api-openapi.yml
- filename: thenile-credentials-api-openapi.yml
  format: yaml
  label: Nile Credentials API
  slug: thenile-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-credentials-api-openapi.yml
- filename: thenile-databases-api-openapi.yml
  format: yaml
  label: Nile Databases API
  slug: thenile-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-databases-api-openapi.yml
- filename: thenile-developers-api-openapi.yml
  format: yaml
  label: Nile Developers API
  slug: thenile-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-developers-api-openapi.yml
- filename: thenile-internal-api-openapi.yml
  format: yaml
  label: Nile Internal API
  slug: thenile-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-internal-api-openapi.yml
- filename: thenile-tenants-api-openapi.yml
  format: yaml
  label: Nile Tenants API
  slug: thenile-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-tenants-api-openapi.yml
- filename: thenile-users-api-openapi.yml
  format: yaml
  label: Nile Users API
  slug: thenile-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-users-api-openapi.yml
- filename: thenile-workspaces-api-openapi.yml
  format: yaml
  label: Nile Workspaces API
  slug: thenile-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Thenile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nile secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nile
provider_slug: thenile
scheme_count: 2
schemes:
- description: Session token stored in a cookie after user signs in, prefixed with __Secure if on https
  in: cookie
  name: sessionCookie
  parameter: nile-auth.session-token
  sources:
  - openapi/thenile-auth-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: jwtBearerAuth
  scheme: bearer
  sources:
  - openapi/thenile-database-openapi.yml
  - openapi/thenile-global-openapi.yml
  type: http
slug: thenile-authentication
source_filename: thenile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/thenile-auth-openapi.yml, openapi/thenile-database-openapi.yml, openapi/thenile-global-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: nile-auth.session-token\n  description: Session token stored in a cookie after user signs in, prefixed with __Secure\n    if on https\n  sources:\n  - openapi/thenile-auth-openapi.yml\n- name: jwtBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/thenile-database-openapi.yml\n  - openapi/thenile-global-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/authentication/thenile-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Database
- PostgreSQL
- Serverless
- Multi-Tenant
- Authentication
- B2B SaaS
---
