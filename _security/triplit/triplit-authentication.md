---
api_key_in: []
api_specs:
- filename: triplit-advanced-api-openapi.yml
  format: yaml
  label: Triplit Advanced API
  slug: triplit-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-advanced-api-openapi.yml
- filename: triplit-auth-api-openapi.yml
  format: yaml
  label: Triplit Auth API
  slug: triplit-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-auth-api-openapi.yml
- filename: triplit-data-api-openapi.yml
  format: yaml
  label: Triplit Data API
  slug: triplit-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-data-api-openapi.yml
- filename: triplit-schema-api-openapi.yml
  format: yaml
  label: Triplit Schema API
  slug: triplit-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-schema-api-openapi.yml
- filename: triplit-system-api-openapi.yml
  format: yaml
  label: Triplit System API
  slug: triplit-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-system-api-openapi.yml
- filename: triplit-webhooks-api-openapi.yml
  format: yaml
  label: Triplit Webhooks API
  slug: triplit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Triplit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Triplit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Triplit
provider_slug: triplit
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Bearer token. Use a Service Token (secret) for admin operations or an Anonymous token for standard user operations.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/triplit-http-api-openapi.yml
  type: http
slug: triplit-authentication
source_filename: triplit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/triplit-http-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token. Use a Service Token (secret) for admin operations or an Anonymous\n    token for standard user operations.\n  sources:\n  - openapi/triplit-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/authentication/triplit-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Real-time
- Sync
- Local-first
- Developer Tools
- TypeScript
- Open Source
---
