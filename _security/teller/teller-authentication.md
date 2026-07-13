---
api_key_in: []
api_specs:
- filename: teller-openapi.yml
  format: yaml
  label: Teller API
  slug: teller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-openapi.yml
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
- FinTech
- Open Banking
- Transactions
- Unified API
---
