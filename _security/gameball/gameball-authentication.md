---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gameball Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gameball secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gameball
provider_slug: gameball
scheme_count: 2
schemes:
- description: Primary account API key sent on every request. Sufficient on its own for standard, non-sensitive endpoints.
  in: header
  name: APIKey
  parameter_name: APIKey
  required: true
  source: https://docs.gameball.co/api-reference/overview/authentication
  type: apiKey
- description: Transaction/secret key. Required alongside APIKey for sensitive operations (transactions, redemptions, holds, coupon burns) and for ALL requests when High Security Mode is enabled. Must only be sent from server-side code.
  in: header
  name: SecretKey
  parameter_name: SecretKey
  required: false
  source: https://docs.gameball.co/api-reference/overview/authentication
  type: apiKey
slug: gameball-authentication
source_filename: gameball-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gameball.co/api-reference/overview/authentication\ndocs: https://docs.gameball.co/api-reference/overview/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Gameball authenticates server-to-server API calls with two API-key headers.\n    APIKey identifies the account/workspace and is required on every request.\n    SecretKey is additionally required on sensitive/transactional operations, and\n    on all operations when \"High Security Mode\" is enabled for the account. No\n    OAuth 2.0 flow or bearer-token grant is used. Requests must originate\n    server-side so the SecretKey is never exposed to the client.\nschemes:\n  - name: APIKey\n    type: apiKey\n    in: header\n    parameter_name: APIKey\n    required: true\n    description: >-\n      Primary account API key sent on every request. Sufficient on its own for\n      standard, non-sensitive endpoints.\n\
  \    source: https://docs.gameball.co/api-reference/overview/authentication\n  - name: SecretKey\n    type: apiKey\n    in: header\n    parameter_name: SecretKey\n    required: false\n    description: >-\n      Transaction/secret key. Required alongside APIKey for sensitive operations\n      (transactions, redemptions, holds, coupon burns) and for ALL requests when\n      High Security Mode is enabled. Must only be sent from server-side code.\n    source: https://docs.gameball.co/api-reference/overview/authentication\nwidget_auth:\n  mechanism: customer hash\n  description: >-\n    Client-side widget/mobile SDK sessions are secured with a per-customer hash\n    (HMAC of the customer id using the account transaction/secret key) generated\n    server-side and passed to the SDK. See the Get Customer Hash operation.\n  docs: https://docs.gameball.co/api-reference/customers/management/get-customer-hash\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/authentication/gameball-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Loyalty
- Rewards
- Gamification
- Customer Engagement
- Retention
- Referrals
- Marketing
- E-commerce
---
