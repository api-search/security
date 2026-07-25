---
api_key_in: []
api_specs:
- filename: papaya-global-authentication-api-openapi.yml
  format: yaml
  label: Papaya Global Authentication API
  slug: papaya-global-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-authentication-api-openapi.yml
- filename: papaya-global-beneficiaries-api-openapi.yml
  format: yaml
  label: Papaya Global Beneficiaries API
  slug: papaya-global-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-beneficiaries-api-openapi.yml
- filename: papaya-global-groups-api-openapi.yml
  format: yaml
  label: Papaya Global Groups API
  slug: papaya-global-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-groups-api-openapi.yml
- filename: papaya-global-payments-api-openapi.yml
  format: yaml
  label: Papaya Global Payments API
  slug: papaya-global-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-payments-api-openapi.yml
- filename: papaya-global-wallets-api-openapi.yml
  format: yaml
  label: Papaya Global Wallets API
  slug: papaya-global-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Papaya Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: Papaya Global secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Papaya Global
provider_slug: papaya-global
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/papaya-global-workforce-payments-api.yml
  type: http
slug: papaya-global-authentication
source_filename: papaya-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/papaya-global-workforce-payments-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/papaya-global-workforce-payments-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/authentication/papaya-global-authentication.yml
summary_line: http · 1 scheme
tags:
- Payroll
- Global Workforce
- HR
- Payments
- Employer of Record
- Contractor Management
- Compliance
---
