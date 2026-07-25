---
api_key_in:
- header
api_specs:
- filename: finicity-openbanking-us-openapi-original.yml
  format: yaml
  label: Finicity Aggregation (Accounts & Transactions) API
  slug: finicity-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/openapi/finicity-openbanking-us-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Finicity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finicity secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finicity
provider_slug: finicity
scheme_count: 2
schemes:
- description: The "Finicity-App-Key" from the developer dashboard
  in: header
  name: FinicityAppKey
  parameter: Finicity-App-Key
  sources:
  - openapi/finicity-openbanking-us-openapi-original.yml
  type: apiKey
- description: A token returned by the `/authentication` API
  in: header
  name: FinicityAppToken
  parameter: Finicity-App-Token
  sources:
  - openapi/finicity-openbanking-us-openapi-original.yml
  type: apiKey
slug: finicity-authentication
source_filename: finicity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/finicity-openbanking-us-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: FinicityAppKey\n  type: apiKey\n  in: header\n  parameter: Finicity-App-Key\n  description: The \"Finicity-App-Key\" from the developer dashboard\n  sources:\n  - openapi/finicity-openbanking-us-openapi-original.yml\n- name: FinicityAppToken\n  type: apiKey\n  in: header\n  parameter: Finicity-App-Token\n  description: A token returned by the `/authentication` API\n  sources:\n  - openapi/finicity-openbanking-us-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/authentication/finicity-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Financial Services
- Data Aggregation
- Open Finance
- Open Banking
- FDX
- United States
- Payments
- Financial Data
---
