---
anonymous_access: false
api_key_in: []
api_specs:
- filename: p2flux-api-cancellation-api-openapi.yml
  format: yaml
  label: P2Flux API Cancellation API
  slug: p2flux-api-cancellation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-cancellation-api-openapi.yml
- filename: p2flux-api-one-time-payments-api-openapi.yml
  format: yaml
  label: P2Flux API One-time payments API
  slug: p2flux-api-one-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-one-time-payments-api-openapi.yml
- filename: p2flux-api-recurring-payments-api-openapi.yml
  format: yaml
  label: P2Flux API Recurring payments API
  slug: p2flux-api-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-recurring-payments-api-openapi.yml
- filename: p2flux-api-refunds-api-openapi.yml
  format: yaml
  label: P2Flux API Refunds API
  slug: p2flux-api-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-refunds-api-openapi.yml
- filename: p2flux-api-service-api-openapi.yml
  format: yaml
  label: P2Flux API Service API
  slug: p2flux-api-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-service-api-openapi.yml
- filename: p2flux-api-subscriptions-api-openapi.yml
  format: yaml
  label: P2Flux API Subscriptions API
  slug: p2flux-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: P2Flux Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: P2Flux API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: P2Flux API
provider_slug: p2flux-api
scheme_count: 0
schemes: []
slug: p2flux-api-authentication
source_filename: p2flux-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: searched\nsource: https://p2flux.com/docs/api.html#auth and https://p2flux.com/.well-known/api-onboarding\napi: P2Flux API\nsummary: >-\n  P2Flux v1 has no API authentication in the conventional sense: no API keys, no bearer\n  tokens, no Authorization header, no cookies and no credentialed CORS. The OpenAPI\n  declares no securitySchemes and an empty top-level security list. Authorization is\n  carried per-request by a signed capability in the JSON body, and — for setting up a\n  subscription or a one-time payment — by the payer's own EIP-712 wallet signature.\nmodel: capability + wallet-signature (no ambient authority)\nsecurity_schemes: []\nmechanisms:\n  - id: signed-capability\n    type: in-body bearer secret\n    description: >-\n      Requests that act on an existing payment, subscription, cancellation or refund\n      carry an opaque capability token in the request body. P2Flux mints each token for\n      exactly one object and HMAC-signs\
  \ it; the signature is what authorizes the call\n      and is verified on every request. Tokens are bound to an exact recipient, amount\n      and period, so a capability can only do what its object allows.\n    token_prefixes:\n      p2f1.: payment intent\n      p2setup2.: subscription setup token\n      p2s2.: subscription capability (authorizes merchant-triggered charges)\n      p2cancel1.: cancel token\n      p2refund1.: refund token\n    handling: >-\n      Treat every capability as a bearer secret: keep it server-side, encrypted at rest,\n      out of URLs, query strings and logs. A p2s2 subscription capability can collect the\n      signed amount once per billing period to the signed recipient.\n  - id: eip-712-payer-signature\n    type: wallet signature\n    description: >-\n      One-time payments and subscription setup require the payer's own EIP-712 typed\n      signature, produced by their wallet. resolveSubscription returns the exact EIP-712\n      payload the customer signs;\
  \ finalizeSubscription exchanges that signature for the\n      p2s2 charge capability. This is the security model, not an onboarding step, and it\n      cannot be automated on the payer's behalf.\n    error_on_failure: INVALID_SIGNATURE (CUSTOMER_ACTION_REQUIRED)\nscopes:\n  model: resource-selection\n  description: >-\n    No account-level scopes. Each capability is scoped to a single object (one payment\n    intent, subscription, cancellation or refund) and cannot exceed what that object\n    authorizes.\n  vocabulary: https://p2flux.com/docs/api.html#auth\nnotes:\n  - health is an unauthenticated liveness endpoint.\n  - Because there is no issued credential, there is nothing to rotate or revoke at the\n    account level; a subscription is stopped on-chain (allowance revocation) or by\n    letting the authorization window lapse.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/authentication/p2flux-api-authentication.yml
summary_line: 0 schemes
tags:
- Payments
- Payment API
- Cryptocurrency
- Stablecoins
- USDC
- Base
- Recurring Payments
- Subscription
- Refunds
- Non-Custodial
---
