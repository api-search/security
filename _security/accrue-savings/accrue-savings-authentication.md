---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accrue-savings-banking-api-openapi.yml
  format: yaml
  label: Accrue Savings Banking API
  slug: accrue-savings-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-banking-api-openapi.yml
- filename: accrue-savings-counterparties-api-openapi.yml
  format: yaml
  label: Accrue Savings Counterparties API
  slug: accrue-savings-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-counterparties-api-openapi.yml
- filename: accrue-savings-counterpartytransfers-api-openapi.yml
  format: yaml
  label: Accrue Savings Counterparty Transfers API
  slug: accrue-savings-counterpartytransfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-counterpartytransfers-api-openapi.yml
- filename: accrue-savings-externaltransactions-api-openapi.yml
  format: yaml
  label: Accrue Savings External Transactions API
  slug: accrue-savings-externaltransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-externaltransactions-api-openapi.yml
- filename: accrue-savings-gifts-api-openapi.yml
  format: yaml
  label: Accrue Savings Gifts API
  slug: accrue-savings-gifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-gifts-api-openapi.yml
- filename: accrue-savings-identity-verification-api-openapi.yml
  format: yaml
  label: Accrue Savings Identity Verification API
  slug: accrue-savings-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-identity-verification-api-openapi.yml
- filename: accrue-savings-payments-api-openapi.yml
  format: yaml
  label: Accrue Savings Payments API
  slug: accrue-savings-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-payments-api-openapi.yml
- filename: accrue-savings-rewards-api-openapi.yml
  format: yaml
  label: Accrue Savings Rewards API
  slug: accrue-savings-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-rewards-api-openapi.yml
- filename: accrue-savings-simulations-api-openapi.yml
  format: yaml
  label: Accrue Savings Simulations API
  slug: accrue-savings-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-simulations-api-openapi.yml
- filename: accrue-savings-sweepstakes-api-openapi.yml
  format: yaml
  label: Accrue Savings Sweepstakes API
  slug: accrue-savings-sweepstakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-sweepstakes-api-openapi.yml
- filename: accrue-savings-users-api-openapi.yml
  format: yaml
  label: Accrue Savings Users API
  slug: accrue-savings-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-users-api-openapi.yml
- filename: accrue-savings-wallets-api-openapi.yml
  format: yaml
  label: Accrue Savings Wallets API
  slug: accrue-savings-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-wallets-api-openapi.yml
- filename: accrue-savings-webhook-topics-api-openapi.yml
  format: yaml
  label: Accrue Savings Webhook Topics API
  slug: accrue-savings-webhook-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-webhook-topics-api-openapi.yml
- filename: accrue-savings-webhooks-api-openapi.yml
  format: yaml
  label: Accrue Savings Webhooks API
  slug: accrue-savings-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-webhooks-api-openapi.yml
- filename: accrue-savings-widgets-api-openapi.yml
  format: yaml
  label: Accrue Savings Widgets API
  slug: accrue-savings-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-widgets-api-openapi.yml
- filename: accrue-savings-linked-accounts-api-openapi.yml
  format: yaml
  label: Accrue Savings Linked Accounts API
  slug: accrue-savings-linked-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-linked-accounts-api-openapi.yml
- filename: accrue-savings-payment-intents-api-openapi.yml
  format: yaml
  label: Accrue Savings Payment Intents API
  slug: accrue-savings-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-payment-intents-api-openapi.yml
- filename: accrue-savings-webhook-events-api-openapi.yml
  format: yaml
  label: Accrue Savings Webhook Events API
  slug: accrue-savings-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-webhook-events-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accrue Savings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accrue Savings declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Accrue Savings
provider_slug: accrue-savings
scheme_count: 2
schemes:
- description: 'Every API call carries `Authorization: Bearer <Client Secret>`. The Client Secret is issued per Client (merchant) and is a backend-only credential — the docs state it must never appear in client-side code and should be rotated periodically. An invalid, missing, or expired token returns HTTP 401.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  source: https://docs.byaccrue.com/api/
  type: http
- description: A Client-ID header accompanies the bearer token and identifies the merchant tenant. It is declared as a required header parameter on all 82 operations in the OpenAPI.
  in: header
  name: clientId
  parameter: Client-ID
  source: openapi/accrue-savings-merchant-api-openapi.yaml
  type: apiKey
slug: accrue-savings-authentication
source_filename: accrue-savings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.byaccrue.com/api/ (Introduction > Authentication) and https://docs.byaccrue.com/getting-started-api\ndocs: https://docs.byaccrue.com/api/\nsummary: Bearer token (the Client Secret) plus a Client-ID header, sent on every request. There is no\n  OAuth, no OIDC, and no mTLS.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: 'Every API call carries `Authorization: Bearer <Client Secret>`. The Client Secret is issued\n    per Client (merchant) and is a backend-only credential — the docs state it must never appear in client-side\n    code and should be rotated periodically. An invalid, missing, or expired token returns HTTP 401.'\n  source: https://docs.byaccrue.com/api/\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: Client-ID\n  description: A Client-ID header accompanies the bearer token and identifies the merchant tenant. It\n   \
  \ is declared as a required header parameter on all 82 operations in the OpenAPI.\n  source: openapi/accrue-savings-merchant-api-openapi.yaml\noauth2: false\nopenid_connect: false\nmutual_tls: false\nerrors:\n  '401': Unauthorized — token invalid, missing, or expired\n  '403': ForbiddenException — observed live on an unauthenticated GET /api/v1/payments\ngaps:\n- The OpenAPI declares NO components.securitySchemes and no top-level or per-operation `security` block.\n  Authentication is expressed only as two required header parameters (Authorization, Client-ID) on each\n  operation, plus prose in the Introduction section. A generator or agent reading the spec alone cannot\n  tell that these are credentials, which is why derive-authentication.py produced nothing for this provider\n  and this file was written from the docs instead.\n- No credential-rotation endpoint, no token expiry semantics, and no scope model are published.\nwebhook_auth:\n  mechanism: signature verification\n  note: The\
  \ getting-started guide instructs integrators to verify webhook signatures with a constant-time\n    comparison, but the signing header name and algorithm are not published in the public docs or the\n    OpenAPI.\n  source: https://docs.byaccrue.com/getting-started-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/authentication/accrue-savings-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Loyalty
- Wallets
- Stored Value
- Rewards
- Banking
- Fintech
- Webhook
- Loyalty & Incentives
---
