---
api_key_in:
- header
api_specs:
- filename: appzen-autonomous-ap-openapi-original.yml
  format: yaml
  label: Autonomous AP API
  slug: autonomous-ap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-autonomous-ap-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appzen Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppZen secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppZen
provider_slug: appzen
scheme_count: 3
schemes:
- description: API key issued by AppZen Support.
  in: header
  name: API Key Header
  parameter: x-api-key
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
- description: Customer identifier issued by AppZen Support.
  in: header
  name: Customer Id Header
  parameter: customer-id
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
- description: Customer key issued by AppZen Support.
  in: header
  name: Customer Key Header
  parameter: customer-key
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
slug: appzen-authentication
source_filename: appzen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/appzen-autonomous-ap-openapi-original.yml\ndocs: https://support.appzen.com/hc/en-us/articles/12905088759571-Authentication-Overview\nguidelines: https://api-docs.appzen.com/api_guidelines.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    AppZen's Autonomous AP public APIs use API-key header authentication. Three\n    values, all issued by the AppZen Support team, must be sent on every request:\n    x-api-key, customer-id, and customer-key. The docs describe the model as\n    \"API key-based authentication (OAuth1.0)\". Every response returns an\n    x-correlation-id header to be quoted to AppZen support when troubleshooting.\nschemes:\n- name: API Key Header\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\n- name: Customer Id Header\n  type: apiKey\n  in: header\n\
  \  parameter: customer-id\n  description: Customer identifier issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\n- name: Customer Key Header\n  type: apiKey\n  in: header\n  parameter: customer-key\n  description: Customer key issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\nresponse_headers:\n- name: x-correlation-id\n  description: Present on every response (success and failure); provide to AppZen Support for troubleshooting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/authentication/appzen-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Finance
- Accounts Payable
- Expense Management
- Invoice Processing
- Spend Audit
- Artificial Intelligence
- ERP Integration
---
