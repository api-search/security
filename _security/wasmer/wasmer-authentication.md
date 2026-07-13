---
api_key_in: []
api_specs:
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Registry GraphQL API
  slug: wasmer-registry-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Packages and Namespaces API
  slug: wasmer-packages-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Apps and Edge Deployments API
  slug: wasmer-apps-edge-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Users and Auth API
  slug: wasmer-users-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wasmer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wasmer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wasmer
provider_slug: wasmer
scheme_count: 1
schemes:
- bearerFormat: wap_*
  description: 'Wasmer API token (wap_* prefix). Create one via `wasmer login` or the dashboard, and supply it as `Authorization: Bearer <token>` or via the WASMER_TOKEN environment variable.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wasmer-openapi.yml
  type: http
slug: wasmer-authentication
source_filename: wasmer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wasmer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: wap_*\n  description: 'Wasmer API token (wap_* prefix). Create one via `wasmer login` or the dashboard,\n    and supply it as `Authorization: Bearer <token>` or via the WASMER_TOKEN environment variable.'\n  sources:\n  - openapi/wasmer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/authentication/wasmer-authentication.yml
summary_line: http · 1 scheme
tags:
- WebAssembly
- Wasm
- Registry
- Edge
- Runtime
---
