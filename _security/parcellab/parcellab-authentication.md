---
api_key_in:
- header
api_specs:
- filename: parcellab-campaigns-api-openapi.yml
  format: yaml
  label: parcelLab Campaigns API
  slug: parcellab-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-campaigns-api-openapi.yml
- filename: parcellab-events-api-openapi.yml
  format: yaml
  label: parcelLab Events API
  slug: parcellab-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-events-api-openapi.yml
- filename: parcellab-orders-api-openapi.yml
  format: yaml
  label: parcelLab Orders API
  slug: parcellab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-orders-api-openapi.yml
- filename: parcellab-place-info-api-openapi.yml
  format: yaml
  label: parcelLab Place Info API
  slug: parcellab-place-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-place-info-api-openapi.yml
- filename: parcellab-promise-api-openapi.yml
  format: yaml
  label: parcelLab Promise API
  slug: parcellab-promise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-promise-api-openapi.yml
- filename: parcellab-returns-api-openapi.yml
  format: yaml
  label: parcelLab Returns API
  slug: parcellab-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-returns-api-openapi.yml
- filename: parcellab-surveys-api-openapi.yml
  format: yaml
  label: parcelLab Surveys API
  slug: parcellab-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-surveys-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parcellab Authentication
name_suffix: Authentication
oauth_flows: []
overview: parcelLab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: parcelLab
provider_slug: parcellab
scheme_count: 1
schemes:
- description: '`Authorization: Parcellab-API-Token <base64(account_id:token)>`. App- generated tokens may instead use the `Bearer <token>` scheme.'
  in: header
  name: parcellabApiToken
  parameter: Authorization
  sources:
  - openapi/parcellab-openapi.yml
  type: apiKey
slug: parcellab-authentication
source_filename: parcellab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parcellab-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: parcellabApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Authorization: Parcellab-API-Token <base64(account_id:token)>`. App- generated\n    tokens may instead use the `Bearer <token>` scheme.'\n  sources:\n  - openapi/parcellab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/authentication/parcellab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Post-Purchase
- E-Commerce
- Tracking
- Returns
- Shipping
- Delivery
- Customer Experience
- Logistics
- Communications
- Germany
---
