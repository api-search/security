---
api_key_in:
- header
api_specs:
- filename: lighthouse-travel-integration-api-openapi.yml
  format: yaml
  label: Lighthouse Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-integration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lighthouse Travel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lighthouse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lighthouse
provider_slug: lighthouse-travel
scheme_count: 1
schemes:
- description: Account-bound API token passed as the X-Oi-Authorization header. Tokens provide access to all subscriptions within the account.
  in: header
  name: LighthouseApiToken
  parameter: X-Oi-Authorization
  sources:
  - openapi/lighthouse-travel-integration-api-openapi.yml
  type: apiKey
slug: lighthouse-travel-authentication
source_filename: lighthouse-travel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lighthouse-travel-integration-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LighthouseApiToken\n  type: apiKey\n  in: header\n  parameter: X-Oi-Authorization\n  description: Account-bound API token passed as the X-Oi-Authorization header. Tokens provide\n    access to all subscriptions within the account.\n  sources:\n  - openapi/lighthouse-travel-integration-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/authentication/lighthouse-travel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Hotels
- Travel
- Revenue Management
- Market Intelligence
- Business Intelligence
- Pricing
- Rate Shopping
- Competitive Intelligence
- Distribution
- Parity
- Channel Manager
- Demand Forecasting
- SaaS
- AI
---
