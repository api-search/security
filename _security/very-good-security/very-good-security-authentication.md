---
api_key_in: []
api_specs:
- filename: very-good-security-vault-openapi-original.yml
  format: yaml
  label: VGS Vault HTTP API
  slug: vgs-vault-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/very-good-security/refs/heads/main/openapi/very-good-security-vault-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Very Good Security Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Very Good Security secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Very Good Security
provider_slug: very-good-security
scheme_count: 2
schemes:
- description: Vault HTTP API default auth — vault access credentials (username/password) generated in the dashboard under the vault's Settings section.
  docs: https://www.verygoodsecurity.com/docs/settings/access-credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/very-good-security-vault-openapi-original.yml
  type: http
- description: Vault API and platform management APIs authenticate via OAuth 2.0 client credentials (service accounts created in the dashboard or via vgs-cli). Access tokens are scoped (aliases:read/write/delete and 150+ platform scopes) AND vault-bound — credentials without an assigned vault get 401 regardless of scopes.
  flows:
    clientCredentials:
      scopes: scopes/very-good-security-scopes.yml
      tokenUrl: https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token
  name: oauth2ClientCredentials
  sources:
  - https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization
  - well-known/very-good-security-openid-configuration.json
  type: oauth2
slug: very-good-security-authentication
source_filename: very-good-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization\ndocs: https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Vault HTTP API default auth — vault access credentials (username/password)\n    generated in the dashboard under the vault's Settings section.\n  docs: https://www.verygoodsecurity.com/docs/settings/access-credentials\n  sources:\n  - openapi/very-good-security-vault-openapi-original.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  description: >-\n    Vault API and platform management APIs authenticate via OAuth 2.0 client\n    credentials (service accounts created in the dashboard or via vgs-cli).\n    Access tokens are scoped (aliases:read/write/delete\
  \ and 150+ platform scopes)\n    AND vault-bound — credentials without an assigned vault get 401 regardless\n    of scopes.\n  flows:\n    clientCredentials:\n      tokenUrl: https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token\n      scopes: scopes/very-good-security-scopes.yml\n  sources:\n  - https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization\n  - well-known/very-good-security-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/very-good-security/refs/heads/main/authentication/very-good-security-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Data Security
- Tokenization
- Payments
- Vault
- PCI Compliance
- Data Privacy
- Card Management
- Network Tokens
- Security
---
