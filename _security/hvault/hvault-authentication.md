---
api_key_in:
- header
api_specs:
- filename: hvault-system-backend-openapi.yml
  format: yaml
  label: Vault System Backend API
  slug: vault-system-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-system-backend-openapi.yml
- filename: hvault-secrets-engines-openapi.yml
  format: yaml
  label: Vault Secrets Engines API
  slug: vault-secrets-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-secrets-engines-openapi.yml
- filename: hvault-auth-methods-openapi.yml
  format: yaml
  label: Vault Auth Methods API
  slug: vault-auth-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-auth-methods-openapi.yml
- filename: hvault-identity-openapi.yml
  format: yaml
  label: Vault Identity API
  slug: vault-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/openapi/hvault-identity-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hvault Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Vault secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashiCorp Vault
provider_slug: hvault
scheme_count: 1
schemes:
- description: Vault authentication token
  in: header
  name: vaultToken
  parameter: X-Vault-Token
  sources:
  - openapi/hvault-auth-methods-openapi.yml
  - openapi/hvault-identity-openapi.yml
  - openapi/hvault-secrets-engines-openapi.yml
  - openapi/hvault-system-backend-openapi.yml
  type: apiKey
slug: hvault-authentication
source_filename: hvault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hvault-auth-methods-openapi.yml, openapi/hvault-identity-openapi.yml, openapi/hvault-secrets-engines-openapi.yml,\n  openapi/hvault-system-backend-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: vaultToken\n  type: apiKey\n  in: header\n  parameter: X-Vault-Token\n  description: Vault authentication token\n  sources:\n  - openapi/hvault-auth-methods-openapi.yml\n  - openapi/hvault-identity-openapi.yml\n  - openapi/hvault-secrets-engines-openapi.yml\n  - openapi/hvault-system-backend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/authentication/hvault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
---
