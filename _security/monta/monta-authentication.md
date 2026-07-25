---
api_key_in: []
api_specs:
- filename: monta-authentication-api-openapi.yml
  format: yaml
  label: Monta Authentication API
  slug: monta-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-authentication-api-openapi.yml
- filename: monta-charge-points-api-openapi.yml
  format: yaml
  label: Monta Charge Points API
  slug: monta-charge-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-charge-points-api-openapi.yml
- filename: monta-charges-api-openapi.yml
  format: yaml
  label: Monta Charges API
  slug: monta-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-charges-api-openapi.yml
- filename: monta-utilities-api-openapi.yml
  format: yaml
  label: Monta Utilities API
  slug: monta-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-utilities-api-openapi.yml
- filename: monta-wallet-transactions-api-openapi.yml
  format: yaml
  label: Monta Wallet Transactions API
  slug: monta-wallet-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-wallet-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Monta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Monta
provider_slug: monta
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 client-credentials bearer token obtained from POST /auth/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/monta-openapi.yml
  type: http
slug: monta-authentication
source_filename: monta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monta-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 client-credentials bearer token obtained from POST /auth/token.\n  sources:\n  - openapi/monta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/authentication/monta-authentication.yml
summary_line: http · 1 scheme
tags:
- EV Charging
- Electric Vehicles
- Charge Points
- Energy
- Mobility
---
