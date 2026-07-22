---
api_key_in:
- header
api_specs:
- filename: wealth-x-connect-openapi.yml
  format: yaml
  label: Wealth-X Connect API
  slug: wealth-x-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-connect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wealth X Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wealth-X secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wealth-X
provider_slug: wealth-x
scheme_count: 3
schemes:
- description: Wealth-X account username, supplied as a request header.
  in: header
  name: wealthxUsername
  parameter: username
  sources:
  - openapi/wealth-x-connect-openapi.yml
  type: apiKey
- description: Wealth-X account password, supplied as a request header.
  in: header
  name: wealthxPassword
  parameter: password
  sources:
  - openapi/wealth-x-connect-openapi.yml
  type: apiKey
- description: Wealth-X API key, supplied as a request header.
  in: header
  name: wealthxApiKey
  parameter: apikey
  sources:
  - openapi/wealth-x-connect-openapi.yml
  type: apiKey
slug: wealth-x-authentication
source_filename: wealth-x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wealth-x-connect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: wealthxUsername\n  type: apiKey\n  in: header\n  parameter: username\n  description: Wealth-X account username, supplied as a request header.\n  sources:\n  - openapi/wealth-x-connect-openapi.yml\n- name: wealthxPassword\n  type: apiKey\n  in: header\n  parameter: password\n  description: Wealth-X account password, supplied as a request header.\n  sources:\n  - openapi/wealth-x-connect-openapi.yml\n- name: wealthxApiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Wealth-X API key, supplied as a request header.\n  sources:\n  - openapi/wealth-x-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/authentication/wealth-x-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Wealth Intelligence
- Data
- UHNW
- Prospecting
- Financial Services
- CRM
- People Data
---
