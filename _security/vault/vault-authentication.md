---
api_key_in:
- header
api_specs:
- filename: vault-auth-methods-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth Methods API
  slug: vault-auth-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-auth-methods-api-openapi.yml
- filename: vault-health-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Health API
  slug: vault-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-health-api-openapi.yml
- filename: vault-leases-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Leases API
  slug: vault-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-leases-api-openapi.yml
- filename: vault-policies-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Policies API
  slug: vault-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-policies-api-openapi.yml
- filename: vault-secrets-config-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets Config API
  slug: vault-secrets-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-secrets-config-api-openapi.yml
- filename: vault-secrets-data-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets Data API
  slug: vault-secrets-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-secrets-data-api-openapi.yml
- filename: vault-secrets-engines-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets Engines API
  slug: vault-secrets-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-secrets-engines-api-openapi.yml
- filename: vault-secrets-metadata-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets Metadata API
  slug: vault-secrets-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/openapi/vault-secrets-metadata-api-openapi.yml
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
