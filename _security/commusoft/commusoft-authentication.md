---
api_key_in:
- header
- query
api_specs:
- filename: commusoft-api-openapi.yml
  format: yaml
  label: Commusoft API
  slug: commusoft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Commusoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commusoft secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Commusoft
provider_slug: commusoft
scheme_count: 2
schemes:
- description: API token obtained from the /getToken endpoint
  in: header
  name: ApiTokenHeader
  parameter: X-Auth-Token
  sources:
  - openapi/commusoft-api-openapi.yml
  type: apiKey
- description: API token passed as a query parameter
  in: query
  name: ApiTokenQuery
  parameter: token
  sources:
  - openapi/commusoft-api-openapi.yml
  type: apiKey
slug: commusoft-authentication
source_filename: commusoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commusoft-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: API token obtained from the /getToken endpoint\n  sources:\n  - openapi/commusoft-api-openapi.yml\n- name: ApiTokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token passed as a query parameter\n  sources:\n  - openapi/commusoft-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/authentication/commusoft-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Field Service Management
- Job Management
- HVAC
- Plumbing
- Trades
- Scheduling
- Invoicing
- Engineers
- Customers
- Service History
---
