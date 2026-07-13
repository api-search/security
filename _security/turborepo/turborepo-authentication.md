---
api_key_in: []
api_specs:
- filename: remote-cache-spec
  format: yaml
  label: Turborepo Remote Cache API
  slug: turborepo-remote-cache-api
  spec_type: OpenAPI
  url: https://turborepo.dev/api/remote-cache-spec
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turborepo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turborepo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Turborepo
provider_slug: turborepo
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Pass your authentication token in the `Authorization` header as `Bearer <token>`.


    For self-hosted implementations, the token format and validation logic is up to the implementer. Common approaches include:

    - Static tokens for simple setups

    - JWT tokens for stateless authentication

    - OAuth2 tokens for integration with identity providers'
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/turborepo-remote-cache-api-openapi.yml
  type: http
slug: turborepo-authentication
source_filename: turborepo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turborepo-remote-cache-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token authentication. Pass your authentication token in the `Authorization` header as `Bearer <token>`.\n\n    For self-hosted implementations, the token format and validation logic is up to the implementer. Common approaches include:\n    - Static tokens for simple setups\n    - JWT tokens for stateless authentication\n    - OAuth2 tokens for integration with identity providers\n  sources:\n  - openapi/turborepo-remote-cache-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turborepo/refs/heads/main/authentication/turborepo-authentication.yml
summary_line: http · 1 scheme
tags:
- Build System
- Monorepo
- JavaScript
- TypeScript
- Caching
- Open Source
- Rust
- Vercel
- Developer Tools
- CI/CD
---
