---
api_key_in:
- header
api_specs:
- filename: parcellab-openapi.yml
  format: yaml
  label: parcelLab API
  slug: parcellab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-openapi.yml
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
