---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coincover-backup-api-openapi.yml
  format: yaml
  label: Coincover Backup API
  slug: coincover-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-backup-api-openapi.yml
- filename: coincover-backups-api-openapi.yml
  format: yaml
  label: Coincover Backups API
  slug: coincover-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-backups-api-openapi.yml
- filename: coincover-key-api-openapi.yml
  format: yaml
  label: Coincover Key API
  slug: coincover-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-key-api-openapi.yml
- filename: coincover-keys-api-openapi.yml
  format: yaml
  label: Coincover Keys API
  slug: coincover-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-keys-api-openapi.yml
- filename: coincover-partner-api-openapi.yml
  format: yaml
  label: Coincover Partner API
  slug: coincover-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-partner-api-openapi.yml
- filename: coincover-secure-api-openapi.yml
  format: yaml
  label: Coincover Secure API
  slug: coincover-secure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-secure-api-openapi.yml
- filename: coincover-verification-api-openapi.yml
  format: yaml
  label: Coincover Verification API
  slug: coincover-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-verification-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Coincover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coincover secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coincover
provider_slug: coincover
scheme_count: 2
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/coincover-backup-api-openapi.yml
  - openapi/coincover-backups-api-openapi.yml
  - openapi/coincover-key-api-openapi.yml
  - openapi/coincover-keys-api-openapi.yml
  - openapi/coincover-partner-api-openapi.yml
  - openapi/coincover-secure-api-openapi.yml
  - openapi/coincover-verification-api-openapi.yml
  type: http
- description: API key for authentication and authorization
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/coincover-backups-api-openapi.yml
  - openapi/coincover-keys-api-openapi.yml
  - openapi/coincover-verification-api-openapi.yml
  type: apiKey
slug: coincover-authentication
source_filename: coincover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/coincover-backup-api-openapi.yml, openapi/coincover-backups-api-openapi.yml,\n  openapi/coincover-key-api-openapi.yml, openapi/coincover-keys-api-openapi.yml, openapi/coincover-partner-api-openapi.yml,\n  openapi/coincover-secure-api-openapi.yml, openapi/coincover-verification-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/coincover-backup-api-openapi.yml\n  - openapi/coincover-backups-api-openapi.yml\n  - openapi/coincover-key-api-openapi.yml\n  - openapi/coincover-keys-api-openapi.yml\n  - openapi/coincover-partner-api-openapi.yml\n  - openapi/coincover-secure-api-openapi.yml\n  - openapi/coincover-verification-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication and authorization\n  sources:\n  - openapi/coincover-backups-api-openapi.yml\n\
  \  - openapi/coincover-keys-api-openapi.yml\n  - openapi/coincover-verification-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/coincover/authentication/coincover-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cryptocurrency
- Security
- Recovery
- Fintech
---
