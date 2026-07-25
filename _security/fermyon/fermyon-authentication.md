---
api_key_in:
- header
api_specs:
- filename: fermyon-accounts-api-openapi.yml
  format: yaml
  label: Fermyon accounts API
  slug: fermyon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-accounts-api-openapi.yml
- filename: fermyon-apps-api-openapi.yml
  format: yaml
  label: Fermyon apps API
  slug: fermyon-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-apps-api-openapi.yml
- filename: fermyon-auth-tokens-api-openapi.yml
  format: yaml
  label: Fermyon auth-tokens API
  slug: fermyon-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-auth-tokens-api-openapi.yml
- filename: fermyon-channels-api-openapi.yml
  format: yaml
  label: Fermyon channels API
  slug: fermyon-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-channels-api-openapi.yml
- filename: fermyon-custom-domains-api-openapi.yml
  format: yaml
  label: Fermyon custom-domains API
  slug: fermyon-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-custom-domains-api-openapi.yml
- filename: fermyon-device-codes-api-openapi.yml
  format: yaml
  label: Fermyon device-codes API
  slug: fermyon-device-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-device-codes-api-openapi.yml
- filename: fermyon-key-value-pairs-api-openapi.yml
  format: yaml
  label: Fermyon key-value-pairs API
  slug: fermyon-key-value-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-pairs-api-openapi.yml
- filename: fermyon-key-value-stores-api-openapi.yml
  format: yaml
  label: Fermyon key-value-stores API
  slug: fermyon-key-value-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-stores-api-openapi.yml
- filename: fermyon-oci-api-openapi.yml
  format: yaml
  label: Fermyon oci API
  slug: fermyon-oci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-oci-api-openapi.yml
- filename: fermyon-payments-api-openapi.yml
  format: yaml
  label: Fermyon payments API
  slug: fermyon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-payments-api-openapi.yml
- filename: fermyon-personal-access-tokens-api-openapi.yml
  format: yaml
  label: Fermyon personal-access-tokens API
  slug: fermyon-personal-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-personal-access-tokens-api-openapi.yml
- filename: fermyon-revisions-api-openapi.yml
  format: yaml
  label: Fermyon revisions API
  slug: fermyon-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-revisions-api-openapi.yml
- filename: fermyon-sql-databases-api-openapi.yml
  format: yaml
  label: Fermyon sql-databases API
  slug: fermyon-sql-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-sql-databases-api-openapi.yml
- filename: fermyon-variable-pairs-api-openapi.yml
  format: yaml
  label: Fermyon variable-pairs API
  slug: fermyon-variable-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-variable-pairs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fermyon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fermyon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fermyon
provider_slug: fermyon
scheme_count: 1
schemes:
- description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/fermyon-openapi.yml
  type: apiKey
slug: fermyon-authentication
source_filename: fermyon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fermyon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/fermyon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/authentication/fermyon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Functions
- WebAssembly
- Serverless
---
