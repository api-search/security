---
api_key_in: []
api_specs:
- filename: teller-accounts-api-openapi.yml
  format: yaml
  label: Teller Accounts API
  slug: teller-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-accounts-api-openapi.yml
- filename: teller-identity-api-openapi.yml
  format: yaml
  label: Teller Identity API
  slug: teller-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-identity-api-openapi.yml
- filename: teller-institutions-api-openapi.yml
  format: yaml
  label: Teller Institutions API
  slug: teller-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-institutions-api-openapi.yml
- filename: teller-transactions-api-openapi.yml
  format: yaml
  label: Teller Transactions API
  slug: teller-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teller Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teller secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teller
provider_slug: teller
scheme_count: 1
schemes:
- description: 'Access token obtained via Teller Connect when a user successfully enrolls their bank account. Must be used together with a Teller client certificate (mTLS). Encoded using HTTP Basic Auth scheme: ACCESS_TOKEN as username, empty password.'
  name: BearerMtls
  scheme: bearer
  sources:
  - openapi/teller-openapi.yml
  type: http
slug: teller-authentication
source_filename: teller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teller-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerMtls\n  type: http\n  scheme: bearer\n  description: 'Access token obtained via Teller Connect when a user successfully enrolls their\n    bank account. Must be used together with a Teller client certificate (mTLS). Encoded using\n    HTTP Basic Auth scheme: ACCESS_TOKEN as username, empty password.'\n  sources:\n  - openapi/teller-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/authentication/teller-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Financial Data
- Fintech
- Open Banking
- Transaction
- Unified-API
---
