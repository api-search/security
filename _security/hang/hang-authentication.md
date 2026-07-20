---
api_key_in:
- header
api_specs:
- filename: hang-partner-api-openapi.yml
  format: yaml
  label: Hang Partner API
  slug: hang-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-partner-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hang Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hang secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hang
provider_slug: hang
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/hang-partner-api-openapi.yml
  type: apiKey
slug: hang-authentication
source_filename: hang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hang-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/hang-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/authentication/hang-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Loyalty
- Rewards
- Membership
- Customer Engagement
- Marketing
- Restaurants
- Point of Sale
- Webhooks
---
