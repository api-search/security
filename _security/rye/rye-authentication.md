---
api_key_in:
- header
api_specs:
- filename: rye-checkout-intents-openapi-original.yml
  format: yaml
  label: Universal Checkout API
  slug: universal-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-checkout-intents-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rye secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rye
provider_slug: rye
scheme_count: 1
schemes:
- description: Rye API key
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/rye-checkout-intents-openapi-original.yml
  type: apiKey
slug: rye-authentication
source_filename: rye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rye-checkout-intents-openapi-original.yml\ndocs: https://rye.com/docs/api-v2/authorization\nnotes: >-\n  API-key auth via the Authorization header. Docs show \"Basic $RYE_API_KEY\" and\n  \"Bearer YOUR_API_KEY\" forms; keys are per-environment (staging vs production keys\n  are not interchangeable). No OAuth2/OIDC - no scope surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Rye API key\n  sources:\n  - openapi/rye-checkout-intents-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/authentication/rye-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Payments
- Agentic Commerce
- AI Agents
- Universal Checkout
- Shopping
---
