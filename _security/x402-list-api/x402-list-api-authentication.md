---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: x402 List API
  slug: x402-list-api
  spec_type: OpenAPI
  url: https://x402-list.com/api/v1/openapi.json
auth_types: []
description: 'There is nothing to authenticate with. x402 List issues no API keys, runs no OAuth, and has no account system — the onboarding descriptor lists an empty credentials array and calls the registration mechanism "open". This is the correct and complete auth profile, not a thin one: the OpenAPI declares no securitySchemes because there are none to declare, and an agent can call every read operation on first contact with zero setup. What replaces authentication is PAYMENT. Past the free quota, and on the two paid write operations, the API answers HTTP 402 with an x402 v2 PaymentRequired envelope and the caller retries carrying a PAYMENT-SIGNATURE header signed by their own wallet. Authorization for the owner-update flow is separate again and is domain-proof based rather than credential based.'
kind: authentication
layout: security
method: searched
name: X402 List Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: x402 List API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: x402 List API
provider_slug: x402-list-api
scheme_count: 0
schemes: []
slug: x402-list-api-authentication
source_filename: x402-list-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://x402-list.com/api/v1/openapi.json (components.securitySchemes is\n  absent and no top-level `security` is declared), the auth prose at\n  https://x402-list.com/api (\"No authentication required for read access\"), the\n  machine-readable https://x402-list.com/.well-known/api-onboarding\n  (account.required false, registration mechanism \"open\", credentials []), and a\n  live unauthenticated GET https://x402-list.com/api/v1/stats that returned\n  HTTP 200 with no credential of any kind.\ndescription: >-\n  There is nothing to authenticate with. x402 List issues no API keys, runs no\n  OAuth, and has no account system — the onboarding descriptor lists an empty\n  credentials array and calls the registration mechanism \"open\". This is the\n  correct and complete auth profile, not a thin one: the OpenAPI declares no\n  securitySchemes because there are none to declare, and an agent can call every\n  read operation\
  \ on first contact with zero setup.\n  What replaces authentication is PAYMENT. Past the free quota, and on the two\n  paid write operations, the API answers HTTP 402 with an x402 v2\n  PaymentRequired envelope and the caller retries carrying a PAYMENT-SIGNATURE\n  header signed by their own wallet. Authorization for the owner-update flow is\n  separate again and is domain-proof based rather than credential based.\nauth_required_for_reads: false\nschemes: []\nsecurityScheme_count: 0\nopenapi_security_declared: false\npayment_authorization:\n  protocol: x402 (HTTP 402 Payment Required), version 2\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  challenge_body_schema: PaymentRequired (components.schemas.PaymentRequired)\n  receipt_header: PAYMENT-RESPONSE\n  network: Base (EVM), USDC\n  applies_to:\n    - Metered reads past 2,000 GET/day per IP ($0.01/request)\n    - POST /api/v1/assess ($0.25)\n    - POST /api/v1/suggestions ($0.10)\n    - POST /api/v1/submit,\
  \ only for free-compute-host URLs ($1.00) or a resubmission within 14 days ($0.50)\n  key_custody: >-\n    The caller signs. The hosted MCP server states in its own initialize\n    instructions that it \"holds no keys\", and the paid MCP tool takes\n    payment_signature_b64 as a tool argument rather than reading a stored wallet.\nownership_authorization:\n  flow: one-time domain proof\n  operations: [requestServiceUpdate, verifyServiceOwnership, reissueOwnershipToken]\n  mechanism: >-\n    requestServiceUpdate returns a one-time token (returned once, never stored in\n    clear). The owner publishes it as a line of a plain-text file at\n    {base_url origin}/.well-known/x402list.txt on the CURRENTLY listed domain,\n    then calls verifyServiceOwnership. The token expires after 72 hours and a\n    verified request still goes to manual human review.\n  docs: https://x402-list.com/api\ndocs: https://x402-list.com/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-list-api/refs/heads/main/authentication/x402-list-api-authentication.yml
summary_line: 0 schemes
tags:
- x402
- crypto
- '402'
- agentic-payments
- API directory
- registry
- AI agents
- blockchain
- developer tools
- uptime monitoring
---
