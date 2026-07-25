---
api_key_in: []
api_specs:
- filename: keygen-artifacts-api-openapi.yml
  format: yaml
  label: Keygen Artifacts API
  slug: keygen-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-artifacts-api-openapi.yml
- filename: keygen-components-api-openapi.yml
  format: yaml
  label: Keygen Components API
  slug: keygen-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-components-api-openapi.yml
- filename: keygen-entitlements-api-openapi.yml
  format: yaml
  label: Keygen Entitlements API
  slug: keygen-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-entitlements-api-openapi.yml
- filename: keygen-licenses-api-openapi.yml
  format: yaml
  label: Keygen Licenses API
  slug: keygen-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-licenses-api-openapi.yml
- filename: keygen-machines-api-openapi.yml
  format: yaml
  label: Keygen Machines API
  slug: keygen-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-machines-api-openapi.yml
- filename: keygen-policies-api-openapi.yml
  format: yaml
  label: Keygen Policies API
  slug: keygen-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-policies-api-openapi.yml
- filename: keygen-processes-api-openapi.yml
  format: yaml
  label: Keygen Processes API
  slug: keygen-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-processes-api-openapi.yml
- filename: keygen-products-api-openapi.yml
  format: yaml
  label: Keygen Products API
  slug: keygen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-products-api-openapi.yml
- filename: keygen-releases-api-openapi.yml
  format: yaml
  label: Keygen Releases API
  slug: keygen-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-releases-api-openapi.yml
- filename: keygen-tokens-api-openapi.yml
  format: yaml
  label: Keygen Tokens API
  slug: keygen-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-tokens-api-openapi.yml
- filename: keygen-users-api-openapi.yml
  format: yaml
  label: Keygen Users API
  slug: keygen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-users-api-openapi.yml
- filename: keygen-webhooks-api-openapi.yml
  format: yaml
  label: Keygen Webhooks API
  slug: keygen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keygen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keygen secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Keygen
provider_slug: keygen
scheme_count: 2
schemes:
- bearerFormat: token
  description: 'Admin, environment, product, user, or license bearer token in the `Authorization: Bearer <token>` header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keygen-openapi.yml
  type: http
- description: HTTP Basic (email:password) used only to generate a user token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/keygen-openapi.yml
  type: http
slug: keygen-authentication
source_filename: keygen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keygen-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: 'Admin, environment, product, user, or license bearer token in the `Authorization:\n    Bearer <token>` header.'\n  sources:\n  - openapi/keygen-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic (email:password) used only to generate a user token.\n  sources:\n  - openapi/keygen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/authentication/keygen-authentication.yml
summary_line: http · 2 schemes
tags:
- Software Licensing
- Entitlements
- License Keys
- Machine Activation
- Distribution
- Auto-Update
---
