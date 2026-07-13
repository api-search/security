---
api_key_in:
- header
api_specs:
- filename: monte-carlo-openapi.yml
  format: yaml
  label: Monte Carlo GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/openapi/monte-carlo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Monte Carlo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monte Carlo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Monte Carlo
provider_slug: monte-carlo
scheme_count: 1
schemes:
- description: 'Monte Carlo expects two headers on each request: `x-mcd-id` (Key ID)

    and `x-mcd-token` (Secret). OpenAPI cannot represent paired header

    auth natively, so `x-mcd-token` must also be sent on every request.'
  in: header
  name: mcdHeaders
  parameter: x-mcd-id
  sources:
  - openapi/monte-carlo-openapi.yml
  type: apiKey
slug: monte-carlo-authentication
source_filename: monte-carlo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monte-carlo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: mcdHeaders\n  type: apiKey\n  in: header\n  parameter: x-mcd-id\n  description: |-\n    Monte Carlo expects two headers on each request: `x-mcd-id` (Key ID)\n    and `x-mcd-token` (Secret). OpenAPI cannot represent paired header\n    auth natively, so `x-mcd-token` must also be sent on every request.\n  sources:\n  - openapi/monte-carlo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/authentication/monte-carlo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Observability
- Data Quality
- Data Reliability
- Data Lake
- Data Warehouse
- Lineage
- Monitoring
- AI Observability
---
