---
api_key_in:
- header
api_specs:
- filename: convex-http-api-openapi.yml
  format: yaml
  label: Convex HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-http-api-openapi.yml
- filename: openapi.json
  format: json
  label: Convex Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.convex.dev/v1/openapi.json
- filename: convex-deployment-platform-api-openapi.yml
  format: yaml
  label: Convex Deployment Platform API
  slug: deployment-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-deployment-platform-api-openapi.yml
- filename: convex-asyncapi.yml
  format: yaml
  label: Convex Sync Protocol
  slug: sync-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/asyncapi/convex-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Convex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convex secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convex
provider_slug: convex
scheme_count: 2
schemes:
- description: 'Authorization header using a deployment key, Team Access Token, or OAuth Application Token. The token must be prefixed with the string "Convex " (e.g. "Authorization: Convex prod:abc123..."). Deployment keys are created in the dashboard or via the Management API.'
  in: header
  name: convexAuth
  parameter: Authorization
  sources:
  - openapi/convex-deployment-platform-api-openapi.yml
  - openapi/convex-http-api-openapi.yml
  type: apiKey
- description: Bearer token from the application's configured authentication provider (e.g. Auth0, Clerk). Used for user-level authorization of function calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/convex-http-api-openapi.yml
  - openapi/convex-management-api-openapi.yml
  type: http
slug: convex-authentication
source_filename: convex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convex-deployment-platform-api-openapi.yml, openapi/convex-http-api-openapi.yml,\n  openapi/convex-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: convexAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authorization header using a deployment key, Team Access Token, or OAuth Application\n    Token. The token must be prefixed with the string \"Convex \" (e.g. \"Authorization: Convex\n    prod:abc123...\"). Deployment keys are created in the dashboard or via the Management API.'\n  sources:\n  - openapi/convex-deployment-platform-api-openapi.yml\n  - openapi/convex-http-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from the application's configured authentication provider (e.g.\n    Auth0, Clerk). Used for user-level authorization of function calls.\n  sources:\n  - openapi/convex-http-api-openapi.yml\n\
  \  - openapi/convex-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/authentication/convex-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Backend
- Database
- Functions
- Real-Time
- Reactive
- Serverless
- TypeScript
---
