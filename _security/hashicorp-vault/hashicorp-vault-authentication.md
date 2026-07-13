---
api_key_in:
- header
api_specs:
- filename: hashicorp-vault-openapi.yml
  format: yaml
  label: HashiCorp Vault HTTP API
  slug: vault-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-vault/refs/heads/main/openapi/hashicorp-vault-openapi.yml
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
