---
api_key_in: []
api_specs:
- filename: keyvault.json
  format: json
  label: Azure Key Vault API
  slug: azure-key-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/keyvault/resource-manager/Microsoft.KeyVault/stable/2023-02-01/keyvault.json
- filename: keyvault.json
  format: json
  label: Azure Key Vault Data Plane API
  slug: azure-key-vault-data-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/keyvault/data-plane/Microsoft.KeyVault/stable/7.4/keyvault.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Key Vault Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Key Vault secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 authentication. Requires an access token scoped to the Key Vault resource.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/azure-key-vault-data-plane-openapi.yml
  type: oauth2
slug: microsoft-azure-key-vault-authentication
source_filename: microsoft-azure-key-vault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-key-vault-data-plane-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 authentication. Requires an access token scoped\n    to the Key Vault resource.\n  sources:\n  - openapi/azure-key-vault-data-plane-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/authentication/microsoft-azure-key-vault-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
---
