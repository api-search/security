---
api_key_in:
- header
auth_types:
- apiKey
description: BILL uses a session/token model, not OAuth. The BILL AP/AR/network APIs use a developer key (devKey) plus a session token (sessionId) obtained from POST /v3/login; both are sent as headers on every subsequent call. The BILL Spend & Expense (formerly Divvy) API uses a separate Spend & Expense API token, sent as the apiToken header, with no API login step.
kind: authentication
layout: security
method: searched
name: Divvy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Divvy secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Divvy
provider_slug: divvy
scheme_count: 3
schemes:
- applies_to: BILL Spend & Expense (Divvy) API endpoints
  docs: https://developer.bill.com/docs/authentication-with-api-token
  in: header
  name: SpendExpenseApiToken
  note: Generated in the BILL Spend & Expense product; no /v3/login required.
  parameter: apiToken
  type: apiKey
- applies_to: BILL AP, AR, BILL network, and webhook APIs
  detail: sessionId is created via POST /v3/login (username, password, organizationId, devKey). Standard sessions expire after 35 minutes of inactivity; AP/AR sync token sessions last 48 hours. MFA-trusted sessions are supported via rememberMeId + device.
  docs: https://developer.bill.com/docs/bill-keys-tokens
  in: header
  name: DevKeyAndSession
  parameters:
  - devKey
  - sessionId
  type: apiKey
- applies_to: Partner-level operations (POST /v3/partner/login)
  docs: https://developer.bill.com/reference/partnerlogin
  in: header
  name: PartnerAppKey
  parameters:
  - appKey
  - sessionId
  type: apiKey
slug: divvy-authentication
source_filename: divvy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://developer.bill.com/docs/bill-keys-tokens and\n  https://developer.bill.com/docs/authentication-with-api-token — Divvy is now\n  BILL Spend & Expense; its API is delivered through the BILL developer platform.\ndocs: https://developer.bill.com/docs/bill-keys-tokens\ndescription: >-\n  BILL uses a session/token model, not OAuth. The BILL AP/AR/network APIs use a\n  developer key (devKey) plus a session token (sessionId) obtained from\n  POST /v3/login; both are sent as headers on every subsequent call. The BILL\n  Spend & Expense (formerly Divvy) API uses a separate Spend & Expense API\n  token, sent as the apiToken header, with no API login step.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\nschemes:\n  - name: SpendExpenseApiToken\n    type: apiKey\n    in: header\n    parameter: apiToken\n    applies_to: BILL Spend & Expense (Divvy) API endpoints\n    docs: https://developer.bill.com/docs/authentication-with-api-token\n\
  \    note: Generated in the BILL Spend & Expense product; no /v3/login required.\n  - name: DevKeyAndSession\n    type: apiKey\n    in: header\n    parameters: [devKey, sessionId]\n    applies_to: BILL AP, AR, BILL network, and webhook APIs\n    docs: https://developer.bill.com/docs/bill-keys-tokens\n    detail: >-\n      sessionId is created via POST /v3/login (username, password, organizationId,\n      devKey). Standard sessions expire after 35 minutes of inactivity; AP/AR sync\n      token sessions last 48 hours. MFA-trusted sessions are supported via\n      rememberMeId + device.\n  - name: PartnerAppKey\n    type: apiKey\n    in: header\n    parameters: [appKey, sessionId]\n    applies_to: Partner-level operations (POST /v3/partner/login)\n    docs: https://developer.bill.com/reference/partnerlogin\nnotes:\n  - No OAuth 2.0 or scopes are documented; scopes/ artifact intentionally omitted.\n  - MFA is supported for BILL v3 API sessions (rememberMeId + device).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divvy/refs/heads/main/authentication/divvy-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Payments
- Spend Management
- Corporate Cards
- Expense Management
- Fintech
- BILL
---
