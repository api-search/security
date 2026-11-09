---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Decadata Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DecaData secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DecaData
provider_slug: decadata-io
scheme_count: 2
schemes:
- description: An x402 v2 payment (base64 JSON) for the requirements in the 402 response's PAYMENT-REQUIRED header
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/decadata-io-openapi.json
  type: apiKey
- description: A funded-trial code from DecaData (ddt_...), instead of a payment, up to its budget
  in: header
  name: trial
  parameter: X-DecaData-Trial
  sources:
  - openapi/decadata-io-openapi.json
  type: apiKey
slug: decadata-io-authentication
source_filename: decadata-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/decadata-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: An x402 v2 payment (base64 JSON) for the requirements in the 402 response's PAYMENT-REQUIRED\n    header\n  sources:\n  - openapi/decadata-io-openapi.json\n- name: trial\n  type: apiKey\n  in: header\n  parameter: X-DecaData-Trial\n  description: A funded-trial code from DecaData (ddt_...), instead of a payment, up to its\n    budget\n  sources:\n  - openapi/decadata-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/decadata-io/authentication/decadata-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Data
- Analytics
- Market Insights
- Real-Time
---
