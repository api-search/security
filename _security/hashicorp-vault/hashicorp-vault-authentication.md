---
api_key_in:
- header
api_specs:
- filename: hashicorp-vault-auth-approle-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - AppRole API
  slug: hashicorp-vault-auth-approle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-approle-api-openapi.yml
- filename: hashicorp-vault-auth-token-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - Token API
  slug: hashicorp-vault-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-token-api-openapi.yml
- filename: hashicorp-vault-auth-userpass-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Auth - Userpass API
  slug: hashicorp-vault-auth-userpass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-auth-userpass-api-openapi.yml
- filename: hashicorp-vault-identity-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Identity API
  slug: hashicorp-vault-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-identity-api-openapi.yml
- filename: hashicorp-vault-leases-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Leases API
  slug: hashicorp-vault-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-leases-api-openapi.yml
- filename: hashicorp-vault-policy-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Policy API
  slug: hashicorp-vault-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-policy-api-openapi.yml
- filename: hashicorp-vault-secrets-kv-v2-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets - KV v2 API
  slug: hashicorp-vault-secrets-kv-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-secrets-kv-v2-api-openapi.yml
- filename: hashicorp-vault-secrets-transit-api-openapi.yml
  format: yaml
  label: HashiCorp Vault Secrets - Transit API
  slug: hashicorp-vault-secrets-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-secrets-transit-api-openapi.yml
- filename: hashicorp-vault-system-api-openapi.yml
  format: yaml
  label: HashiCorp Vault System API
  slug: hashicorp-vault-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-system-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hashicorp Vault Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Vault secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashiCorp Vault
provider_slug: hashicorp-vault
scheme_count: 1
schemes:
- description: Vault client token
  in: header
  name: VaultToken
  parameter: X-Vault-Token
  sources:
  - openapi/hashicorp-vault-openapi.yml
  type: apiKey
slug: hashicorp-vault-authentication
source_filename: hashicorp-vault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hashicorp-vault-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VaultToken\n  type: apiKey\n  in: header\n  parameter: X-Vault-Token\n  description: Vault client token\n  sources:\n  - openapi/hashicorp-vault-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/authentication/hashicorp-vault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- Encryption
- Infrastructure
- Secrets Management
- Security
---
