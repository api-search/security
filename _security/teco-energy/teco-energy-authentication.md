---
api_key_in: []
api_specs:
- filename: teco-energy-accounts-api-openapi.yml
  format: yaml
  label: TECO Energy Accounts API
  slug: teco-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-accounts-api-openapi.yml
- filename: teco-energy-billing-api-openapi.yml
  format: yaml
  label: TECO Energy Billing API
  slug: teco-energy-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-billing-api-openapi.yml
- filename: teco-energy-energy-usage-api-openapi.yml
  format: yaml
  label: TECO Energy Energy Usage API
  slug: teco-energy-energy-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-energy-usage-api-openapi.yml
- filename: teco-energy-outages-api-openapi.yml
  format: yaml
  label: TECO Energy Outages API
  slug: teco-energy-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-outages-api-openapi.yml
- filename: teco-energy-service-requests-api-openapi.yml
  format: yaml
  label: TECO Energy Service Requests API
  slug: teco-energy-service-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-service-requests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teco Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: TECO Energy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TECO Energy
provider_slug: teco-energy
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teco-energy-account-openapi.yml
  - openapi/teco-energy-outage-openapi.yml
  type: http
slug: teco-energy-authentication
source_filename: teco-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teco-energy-account-openapi.yml, openapi/teco-energy-outage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/teco-energy-account-openapi.yml\n  - openapi/teco-energy-outage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/authentication/teco-energy-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Electric
- Natural Gas
- Smart Grid
- Tampa Bay
- Fortune 1000
---
