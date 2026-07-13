---
api_key_in: []
api_specs:
- filename: trpc-openapi.yml
  format: yaml
  label: tRPC HTTP Protocol
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trpc/refs/heads/main/openapi/trpc-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trpc Authentication
name_suffix: Authentication
oauth_flows: []
overview: tRPC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: tRPC
provider_slug: trpc
scheme_count: 1
schemes:
- description: Bearer token for protected procedures
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/trpc-openapi.yml
  type: http
slug: trpc-authentication
source_filename: trpc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trpc-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for protected procedures\n  sources:\n  - openapi/trpc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trpc/refs/heads/main/authentication/trpc-authentication.yml
summary_line: http · 1 scheme
tags:
- API Composition
- API Framework
- BFF
- End-to-End Type Safety
- RPC
- TypeScript
---
