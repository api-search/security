---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Zuper REST API
  slug: zuper-rest-api
  spec_type: OpenAPI
  url: https://developers.zuper.co/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zuper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zuper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zuper
provider_slug: zuper
scheme_count: 1
schemes:
- description: API key generated from Zuper Settings > Developer Hub > API Keys
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/zuper-rest-api-openapi.yml
  type: apiKey
slug: zuper-authentication
source_filename: zuper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zuper-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from Zuper Settings > Developer Hub > API Keys\n  sources:\n  - openapi/zuper-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/authentication/zuper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Field Service Management
- Scheduling
- Dispatching
- Invoicing
- Timesheets
- Asset Management
- Work Orders
- Customer Management
- Inventory
- Projects
---
