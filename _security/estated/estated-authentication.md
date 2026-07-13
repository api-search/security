---
api_key_in:
- query
api_specs:
- filename: estated-property-data-api-openapi.yml
  format: yaml
  label: Estated Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/openapi/estated-property-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Estated Authentication
name_suffix: Authentication
oauth_flows: []
overview: Estated secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Estated
provider_slug: estated
scheme_count: 1
schemes:
- in: query
  name: tokenQuery
  parameter: token
  sources:
  - openapi/estated-property-data-api-openapi.yml
  type: apiKey
slug: estated-authentication
source_filename: estated-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/estated-property-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/estated-property-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/authentication/estated-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Property Data
- Real Estate
- Property Records
- Assessor
- Parcels
- APN
- FIPS
- Deeds
- AVM
- Valuation
- Boundaries
- GIS
- Owner Of Record
- Tax Assessment
---
