---
api_key_in:
- query
api_specs:
- filename: clickpost-openapi.yml
  format: yaml
  label: ClickPost API
  slug: clickpost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickpost/refs/heads/main/openapi/clickpost-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clickpost Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickPost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClickPost
provider_slug: clickpost
scheme_count: 1
schemes:
- description: ClickPost API token passed as a query parameter or header.
  in: query
  name: apiKeyAuth
  parameter: key
  sources:
  - openapi/clickpost-openapi.yml
  type: apiKey
slug: clickpost-authentication
source_filename: clickpost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clickpost-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: ClickPost API token passed as a query parameter or header.\n  sources:\n  - openapi/clickpost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickpost/refs/heads/main/authentication/clickpost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Carriers
- Delivery
- E-Commerce Logistics
- Logistics
- Returns
- Shipping
- Supply Chain
- Tracking
---
