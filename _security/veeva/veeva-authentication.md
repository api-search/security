---
api_key_in:
- header
api_specs:
- filename: veeva-vault-openapi.yml
  format: yaml
  label: Veeva Vault Platform API
  slug: veeva-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-vault-openapi.yml
- filename: veeva-vault-openapi.yml
  format: yaml
  label: Veeva Vault Query Language (VQL) API
  slug: veeva-vault-query-language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-vault-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veeva Authentication
name_suffix: Authentication
oauth_flows: []
overview: veeva secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: veeva
provider_slug: veeva
scheme_count: 1
schemes:
- description: Vault Session ID from /auth endpoint
  in: header
  name: VaultSession
  parameter: Authorization
  sources:
  - openapi/veeva-vault-openapi.yml
  type: apiKey
slug: veeva-authentication
source_filename: veeva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veeva-vault-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VaultSession\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Vault Session ID from /auth endpoint\n  sources:\n  - openapi/veeva-vault-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/authentication/veeva-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
