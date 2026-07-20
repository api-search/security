---
api_key_in:
- body
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Authorizenet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Authorize.net secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Authorize.net
provider_slug: authorizenet
scheme_count: 3
schemes:
- description: Primary authentication for the transaction gateway. Every request carries a merchantAuthentication element with the merchant API Login ID (name) and Transaction Key. Sandbox and production use distinct credentials.
  docs: https://developer.authorize.net/api/reference/index.html#authentication
  fields:
  - name
  - transactionKey
  in: body
  name: merchantAuthentication
  type: apiKey
- description: A Signature Key (HMAC-SHA512) is used to verify transaction hashes and to sign/verify webhook payloads (X-ANET-Signature header). Configured in the Merchant Interface.
  in: body-hash
  name: signatureKey
  type: apiKey
- description: OAuth 2.0 is available for partner and Accept integrations, allowing a merchant to grant a partner application access without sharing raw API credentials. Demonstrated in the official oauth-sample-app.
  flow: authorizationCode
  name: oauth2
  sample: https://github.com/AuthorizeNet/oauth-sample-app
  type: oauth2
slug: authorizenet-authentication
source_filename: authorizenet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.authorize.net/api/reference/index.html and https://github.com/AuthorizeNet/oauth-sample-app\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [body]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: merchantAuthentication\n  type: apiKey\n  in: body\n  description: >-\n    Primary authentication for the transaction gateway. Every request carries a\n    merchantAuthentication element with the merchant API Login ID (name) and Transaction\n    Key. Sandbox and production use distinct credentials.\n  fields:\n    - name          # API Login ID\n    - transactionKey  # Transaction Key\n  docs: https://developer.authorize.net/api/reference/index.html#authentication\n- name: signatureKey\n  type: apiKey\n  in: body-hash\n  description: >-\n    A Signature Key (HMAC-SHA512) is used to verify transaction hashes and to sign/verify\n    webhook payloads (X-ANET-Signature header). Configured in the Merchant Interface.\n\
  - name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    OAuth 2.0 is available for partner and Accept integrations, allowing a merchant to\n    grant a partner application access without sharing raw API credentials. Demonstrated\n    in the official oauth-sample-app.\n  sample: https://github.com/AuthorizeNet/oauth-sample-app\nnotes: >-\n  The gateway is credential-based (API Login ID + Transaction Key) rather than OAuth-scope\n  based for most integrations; there is no public OAuth scopes reference, so no scopes/\n  artifact is emitted. OAuth 2.0 covers partner delegation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authorizenet/refs/heads/main/authentication/authorizenet-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Payments
- Payment Gateway
- Credit Cards
- eCommerce
- Recurring Billing
- Fraud Detection
- Webhooks
- Financial Services
---
