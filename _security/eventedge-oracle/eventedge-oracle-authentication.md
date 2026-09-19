---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eventedge-oracle-cancellation-api-openapi.yml
  format: yaml
  label: EventEdge Oracle Cancellation API
  slug: eventedge-oracle-cancellation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-cancellation-api-openapi.yml
- filename: eventedge-oracle-one-time-payments-api-openapi.yml
  format: yaml
  label: EventEdge Oracle One-time payments API
  slug: eventedge-oracle-one-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-one-time-payments-api-openapi.yml
- filename: eventedge-oracle-recurring-payments-api-openapi.yml
  format: yaml
  label: EventEdge Oracle Recurring payments API
  slug: eventedge-oracle-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-recurring-payments-api-openapi.yml
- filename: eventedge-oracle-refunds-api-openapi.yml
  format: yaml
  label: EventEdge Oracle Refunds API
  slug: eventedge-oracle-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-refunds-api-openapi.yml
- filename: eventedge-oracle-service-api-openapi.yml
  format: yaml
  label: EventEdge Oracle Service API
  slug: eventedge-oracle-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-service-api-openapi.yml
- filename: eventedge-oracle-subscriptions-api-openapi.yml
  format: yaml
  label: EventEdge Oracle Subscriptions API
  slug: eventedge-oracle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/openapi/eventedge-oracle-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Eventedge Oracle Authentication
name_suffix: Authentication
oauth_flows: []
overview: EventEdge Oracle declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: EventEdge Oracle
provider_slug: eventedge-oracle
scheme_count: 0
schemes: []
slug: eventedge-oracle-authentication
source_filename: eventedge-oracle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: derived\nsource: openapi/eventedge-oracle-openapi.json + live 402 probe of /v1/market/pulse\nsummary: >-\n  No conventional API authentication. The OpenAPI declares security: [] on every\n  operation and no securitySchemes — there is no API key, OAuth, or bearer token and\n  no signup. Access to paid data is instead gated by the x402 payment protocol: an\n  unpaid request to a paid route returns HTTP 402 with a payment-required challenge,\n  and the caller settles a USDC micropayment on Base (eip155:8453) to receive the\n  payload.\nschemes: []\naccess_control:\n  model: x402-payment-gated\n  http_status_on_challenge: 402\n  challenge_header: payment-required\n  network: eip155:8453\n  asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n  asset_name: USD Coin (USDC)\n  pay_to: '0x3a2F36D61c9BB3b3ee72426e2B6b58d774605B5e'\n  scheme: exact\n  max_timeout_seconds: 300\n  free_routes:\n    - /v1/teasers\n    - /v1/agent/preflight\n  evidence:\n\
  \    url: https://edge.arakelproof.space/v1/market/pulse\n    http_status: 402\n    fetched: '2026-09-15'\nnote: >-\n  Authentication (proving who you are) is intentionally absent; authorization is\n  economic (proving you paid). Documented via the x402 well-known manifest and the\n  live 402 challenge, not a securityScheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventedge-oracle/refs/heads/main/authentication/eventedge-oracle-authentication.yml
summary_line: 0 schemes
tags:
- Prediction Markets
- x402
- AI Agents
- Polymarket
- Kalshi
- market-context
- Decision Support
- Finance
---
