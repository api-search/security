---
api_key_in:
- header
api_specs:
- filename: evari-quotes-api-openapi.yml
  format: yaml
  label: Evari Quotes API
  slug: evari-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evari/refs/heads/main/openapi/evari-quotes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Evari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evari secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evari
provider_slug: evari
scheme_count: 1
schemes:
- in: header
  name: undefined
  parameter: Authorization
  sources:
  - openapi/evari-quotes-api-openapi.yml
  type: apiKey
slug: evari-authentication
source_filename: evari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/evari-quotes-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: undefined\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/evari-quotes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evari/refs/heads/main/authentication/evari-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Australia
- Insurtech
- Policy Administration
- Core Systems
- Property and Casualty
- Underwriting
- Claims
- Broker
- MGA
- Artificial Intelligence
- Quoting
- Endorsements
---
