---
api_key_in: []
api_specs:
- filename: google-vault-exports-api-openapi.yml
  format: yaml
  label: Google Vault Exports API
  slug: google-vault-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-exports-api-openapi.yml
- filename: google-vault-heldaccounts-api-openapi.yml
  format: yaml
  label: Google Vault HeldAccounts API
  slug: google-vault-heldaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-heldaccounts-api-openapi.yml
- filename: google-vault-holds-api-openapi.yml
  format: yaml
  label: Google Vault Holds API
  slug: google-vault-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-holds-api-openapi.yml
- filename: google-vault-matters-api-openapi.yml
  format: yaml
  label: Google Vault Matters API
  slug: google-vault-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-matters-api-openapi.yml
- filename: google-vault-operations-api-openapi.yml
  format: yaml
  label: Google Vault Operations API
  slug: google-vault-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-operations-api-openapi.yml
- filename: google-vault-savedqueries-api-openapi.yml
  format: yaml
  label: Google Vault SavedQueries API
  slug: google-vault-savedqueries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-savedqueries-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Vault Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Vault secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Vault
provider_slug: google-vault
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  sources:
  - openapi/google-vault-openapi.yml
  type: oauth2
slug: google-vault-authentication
source_filename: google-vault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-vault-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: googleOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-vault-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/authentication/google-vault-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
