---
api_key_in: []
auth_types:
- token
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bkash Authentication
name_suffix: Authentication
oauth_flows: []
overview: bKash secures its APIs with token and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: bKash
provider_slug: bkash
scheme_count: 2
schemes:
- credentials:
  - username
  - password
  - app_key
  - app_secret
  grant_endpoint: '{base_URL}/tokenized/checkout/token/grant'
  header: Authorization
  in: header
  name: GrantToken
  refresh: Call Refresh Token API (or Grant Token again) before the token expires (around the 50th/55th minute). Do not call more than twice within an hour or the caller is blocked for one hour.
  refresh_endpoint: '{base_URL}/tokenized/checkout/token/refresh'
  token_lifetime_seconds: 3600
  type: token
  value: id_token returned by Grant Token API
- applied_to: All payment/agreement/refund operations alongside the Authorization token.
  header: X-App-Key
  in: header
  name: AppKey
  type: apiKey
  value: Application Key shared by bKash during onboarding
slug: bkash-authentication
source_filename: bkash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.bka.sh/docs/token-management-overview.md\ndocs: https://developer.bka.sh/docs/token-management-overview-1.md\nsummary:\n  types: [token, apiKey]\n  model: >-\n    App-credential bootstrap then bearer-style id_token. Merchant obtains an\n    id_token via the Grant Token API using onboarding credentials (username,\n    password, app_key, app_secret), then sends that token in the Authorization\n    header plus X-App-Key on every payment API call. No standard OAuth2/OIDC\n    discovery is published; the token scheme is bKash-proprietary.\nschemes:\n- name: GrantToken\n  type: token\n  in: header\n  header: Authorization\n  value: id_token returned by Grant Token API\n  token_lifetime_seconds: 3600\n  refresh: >-\n    Call Refresh Token API (or Grant Token again) before the token expires\n    (around the 50th/55th minute). Do not call more than twice within an hour or\n    the caller is blocked for one hour.\n\
  \  grant_endpoint: '{base_URL}/tokenized/checkout/token/grant'\n  refresh_endpoint: '{base_URL}/tokenized/checkout/token/refresh'\n  credentials: [username, password, app_key, app_secret]\n- name: AppKey\n  type: apiKey\n  in: header\n  header: X-App-Key\n  value: Application Key shared by bKash during onboarding\n  applied_to: All payment/agreement/refund operations alongside the Authorization token.\nnotes: >-\n  Credentials (app_key, app_secret, username, password) are issued during bKash\n  merchant onboarding — separate sandbox and production credential sets. Tokens\n  are scoped to the actions permitted for the merchant account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bkash/refs/heads/main/authentication/bkash-authentication.yml
summary_line: token/apiKey · 2 schemes
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- Mobile Financial Services
- Digital Wallet
- Bangladesh
- Checkout
- Webhooks
---
