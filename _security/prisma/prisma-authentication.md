---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Prisma Data Platform API
  slug: prisma-data-platform-api
  spec_type: OpenAPI
  url: https://api.cloud.prisma.io/openapi.json
- filename: prisma-accelerate-openapi.yml
  format: yaml
  label: Prisma Accelerate API
  slug: prisma-accelerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-accelerate-openapi.yml
- filename: prisma-pulse-openapi.yml
  format: yaml
  label: Prisma Pulse API
  slug: prisma-pulse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-pulse-openapi.yml
- filename: prisma-postgres-management-openapi.yml
  format: yaml
  label: Prisma Postgres Management API
  slug: prisma-postgres-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-postgres-management-openapi.yml
- filename: prisma-client-openapi.yml
  format: yaml
  label: Prisma Client API
  slug: prisma-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-client-openapi.yml
- filename: prisma-optimize-openapi.yml
  format: yaml
  label: Prisma Optimize API
  slug: prisma-optimize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-optimize-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prisma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prisma secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prisma
provider_slug: prisma
scheme_count: 2
schemes:
- description: API key for Accelerate authentication, provided as a Bearer token. Generated from the Prisma Data Platform Console for each environment.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/prisma-accelerate-openapi.yml
  - openapi/prisma-optimize-openapi.yml
  - openapi/prisma-pulse-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Authentication via service token or OAuth 2.0 access token. Service tokens are created in the Prisma Console under workspace settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prisma-data-platform-openapi.yml
  - openapi/prisma-postgres-management-openapi.yml
  type: http
slug: prisma-authentication
source_filename: prisma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prisma-accelerate-openapi.yml, openapi/prisma-data-platform-openapi.yml, openapi/prisma-optimize-openapi.yml,\n  openapi/prisma-postgres-management-openapi.yml, openapi/prisma-pulse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for Accelerate authentication, provided as a Bearer token. Generated\n    from the Prisma Data Platform Console for each environment.\n  sources:\n  - openapi/prisma-accelerate-openapi.yml\n  - openapi/prisma-optimize-openapi.yml\n  - openapi/prisma-pulse-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Authentication via service token or OAuth 2.0 access token. Service tokens are\n    created in the Prisma Console under workspace settings.\n  sources:\n  - openapi/prisma-data-platform-openapi.yml\n\
  \  - openapi/prisma-postgres-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/authentication/prisma-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
