---
api_key_in: []
api_specs:
- filename: drippay-openapi-original.json
  format: json
  label: Drip API
  slug: drip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drippay/refs/heads/main/openapi/drippay-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drippay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drippay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drippay
provider_slug: drippay
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'API key from Drip Dashboard. Format: `sk_live_...` or `sk_test_...`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drippay-openapi-original.json
  type: http
slug: drippay-authentication
source_filename: drippay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/drippay-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'API key from Drip Dashboard. Format: `sk_live_...` or `sk_test_...`'\n  sources:\n  - openapi/drippay-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drippay/refs/heads/main/authentication/drippay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Billing
- Usage-Based Billing
- Metering
- Monetization
- Payments
- AI Agents
- Developer Tools
- Webhooks
- MCP
- CRM
- Sales Automation
---
