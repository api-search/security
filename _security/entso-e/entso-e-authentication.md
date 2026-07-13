---
api_key_in:
- query
api_specs:
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Day-Ahead Prices API
  slug: entso-e-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Load API
  slug: entso-e-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Generation API
  slug: entso-e-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Balancing API
  slug: entso-e-balancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Transmission API
  slug: entso-e-transmission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Entso E Authentication
name_suffix: Authentication
oauth_flows: []
overview: ENTSO-E secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ENTSO-E
provider_slug: entso-e
scheme_count: 1
schemes:
- description: Free personal token issued after registering on the Transparency Platform and requesting Restful API access from transparency@entsoe.eu.
  in: query
  name: securityToken
  parameter: securityToken
  sources:
  - openapi/entso-e-openapi.yml
  type: apiKey
slug: entso-e-authentication
source_filename: entso-e-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/entso-e-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: securityToken\n  type: apiKey\n  in: query\n  parameter: securityToken\n  description: Free personal token issued after registering on the Transparency Platform and\n    requesting Restful API access from transparency@entsoe.eu.\n  sources:\n  - openapi/entso-e-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/authentication/entso-e-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Electricity
- Energy
- Energy Markets
- Day-Ahead Prices
- Balancing
- Transmission
- Grid Data
- Europe
---
