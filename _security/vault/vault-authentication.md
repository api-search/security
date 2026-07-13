---
api_key_in:
- header
api_specs:
- filename: vault-kv-openapi.yml
  format: yaml
  label: HashiCorp Vault KV Secrets Engine API
  slug: vault-kv
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-kv-openapi.yml
- filename: vault-sys-openapi.yml
  format: yaml
  label: HashiCorp Vault System Backend API
  slug: vault-sys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-sys-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vault Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Vault secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashiCorp Vault
provider_slug: vault
scheme_count: 1
schemes:
- description: Vault token for authenticating API requests. Tokens can be created via login endpoints or the token auth method. The token must have appropriate policy permissions for the requested operations.
  in: header
  name: vaultToken
  parameter: X-Vault-Token
  sources:
  - openapi/vault-kv-openapi.yml
  - openapi/vault-sys-openapi.yml
  type: apiKey
slug: vault-authentication
source_filename: vault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vault-kv-openapi.yml, openapi/vault-sys-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: vaultToken\n  type: apiKey\n  in: header\n  parameter: X-Vault-Token\n  description: Vault token for authenticating API requests. Tokens can be created via login\n    endpoints or the token auth method. The token must have appropriate policy permissions for\n    the requested operations.\n  sources:\n  - openapi/vault-kv-openapi.yml\n  - openapi/vault-sys-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/authentication/vault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- Encryption
- Open Source
- PKI
- Secrets Management
- Security
---
