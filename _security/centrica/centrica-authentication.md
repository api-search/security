---
api_key_in:
- header
- query
api_specs:
- filename: centrica-fieldops-identity-api-openapi.yml
  format: yaml
  label: Centrica FieldOps Identity API
  slug: centrica-fieldops-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrica/refs/heads/main/openapi/centrica-fieldops-identity-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Centrica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centrica secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Centrica
provider_slug: centrica
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/centrica-fieldops-identity-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/centrica-fieldops-identity-api-openapi.yml
  type: apiKey
slug: centrica-authentication
source_filename: centrica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/centrica-fieldops-identity-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/centrica-fieldops-identity-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/centrica-fieldops-identity-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrica/refs/heads/main/authentication/centrica-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Energy Markets
- Ireland
- Field Service
---
