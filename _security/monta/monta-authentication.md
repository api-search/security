---
api_key_in: []
api_specs:
- filename: monta-openapi.yml
  format: yaml
  label: Monta Charge Points
  slug: charge-points
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Charges and Sessions
  slug: charges-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Teams
  slug: teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Wallets and Transactions
  slug: wallets-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Tariffs and Plans
  slug: tariffs-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
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
