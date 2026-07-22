---
api_key_in:
- header
api_specs:
- filename: syntage-openapi-original.yml
  format: yaml
  label: Syntage API
  slug: syntage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syntage/refs/heads/main/openapi/syntage-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Syntage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syntage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Syntage
provider_slug: syntage
scheme_count: 1
schemes:
- description: Your API key is available in the [Production](https://app.syntage.com/settings/api-keys) and [Sandbox](https://app.sandbox.syntage.com/settings/api-keys) dashboards.
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/syntage-openapi-original.yml
  type: apiKey
slug: syntage-authentication
source_filename: syntage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/syntage-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your API key is available in the [Production](https://app.syntage.com/settings/api-keys)\n    and [Sandbox](https://app.sandbox.syntage.com/settings/api-keys) dashboards.\n  sources:\n  - openapi/syntage-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syntage/refs/heads/main/authentication/syntage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Mexico
- Credit Risk
- Financial Data
- KYC
- Compliance
- Invoices
- Factoring
- SAT
---
