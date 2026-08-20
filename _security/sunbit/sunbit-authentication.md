---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sunbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunbit secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sunbit
provider_slug: sunbit
scheme_count: 4
schemes:
- description: Partner/alliance API key issued by Sunbit. Required on every Sunbit Partner API call. Keys are environment-scoped — sandbox and production keys are distinct. The same key is also used as the publishable initializer for the browser SDK (SUNBIT.init sunbitKey), where the secret must never be included.
  environments:
    production: https://api.sunbit.com
    sandbox: https://api-sandbox.sunbit.com
  in: header
  name: sunbit-key
  parameter_name: sunbit-key
  sources:
  - https://docs.sunbit.com/docs/api-integrations/sunbit-pre-qualification
  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk
  type: apiKey
- description: Paired secret issued by Sunbit, sent alongside sunbit-key. Required on the higher-trust server-to-server operations (checkout initialization, void, refund, merchant onboarding, embedded portal login link, reporting) and optional on transaction lookup. Must never be placed in browser/client code.
  in: header
  name: sunbit-secret
  not_required_on:
  - PUT /purchase/api/v1/online-link
  - PUT /purchase/api/v1/payment-estimation
  - POST /epay/api/v1/epay/send-link
  optional_on:
  - GET /epay/api/v1/epay
  parameter_name: sunbit-secret
  required_on:
  - POST /epay/api/v1/epay
  - PUT /epay/api/v1/epay/cancel/{purchaseId}
  - PUT /epay/api/v1/epay/changeAmount/{purchaseId}
  - POST /onboarding/api/v1/location
  - GET /onboarding/api/v1/location/{location}
  - POST /developers-portal-service/api/v2/auth/login-link
  - POST /alliance/api/v1/merchant-authentication
  - GET /reports/api/v1/summary
  - GET /reports/api/v1/detailed
  - GET /reports/api/v1/customer-offer-history
  sources:
  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk
  - https://docs.sunbit.com/docs/onboarding/adding-new-location
  type: apiKey
- description: Short-lived bearer token minted by POST /alliance/api/v1/merchant-authentication for the Payment Path SDK. Exchanged from sunbit-key + sunbit-secret plus a location; returned with an ISO-8601 expiresAt. The docs instruct integrators to treat the token as opaque and not parse it. Used browser-side to initialize the Payment Path module.
  expiry: ISO-8601 expiresAt returned with the token
  name: merchantAuthToken
  scheme: bearer
  sources:
  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-payment-path
  token_endpoint: https://api.sunbit.com/alliance/api/v1/merchant-authentication
  token_endpoint_sandbox: https://api-sandbox.sunbit.com/alliance/api/v1/merchant-authentication
  type: http
- bearerFormat: JWT
  description: Per-transaction JWT returned by the checkout initialization call (POST /epay/api/v1/epay). Handed to the browser and passed to SUNBIT.epay.checkout to open the hosted checkout modal. Carries the retailer/alliance/transaction context and an exp claim; it authorizes one checkout, not the API.
  name: checkoutToken
  scheme: bearer
  sources:
  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk
  type: http
slug: sunbit-authentication
source_filename: sunbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://docs.sunbit.com/docs/overview/getting-started\ndocs:\n- https://docs.sunbit.com/docs/overview/getting-started\n- https://docs.sunbit.com/docs/overview/production-access\n- https://docs.sunbit.com/docs/sdk-integrations/sunbit-payment-path\nnote: >-\n  Derived by reading Sunbit's published developer documentation, not from an OpenAPI\n  document — Sunbit publishes no machine-readable specification. Every scheme below is\n  named verbatim in the docs.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  ip_allowlisting: true\nschemes:\n- name: sunbit-key\n  type: apiKey\n  in: header\n  parameter_name: sunbit-key\n  description: >-\n    Partner/alliance API key issued by Sunbit. Required on every Sunbit Partner API call.\n    Keys are environment-scoped — sandbox and production keys are distinct. The same key is\n    also used as the publishable\
  \ initializer for the browser SDK (SUNBIT.init sunbitKey),\n    where the secret must never be included.\n  environments:\n    sandbox: https://api-sandbox.sunbit.com\n    production: https://api.sunbit.com\n  sources:\n  - https://docs.sunbit.com/docs/api-integrations/sunbit-pre-qualification\n  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk\n- name: sunbit-secret\n  type: apiKey\n  in: header\n  parameter_name: sunbit-secret\n  description: >-\n    Paired secret issued by Sunbit, sent alongside sunbit-key. Required on the higher-trust\n    server-to-server operations (checkout initialization, void, refund, merchant onboarding,\n    embedded portal login link, reporting) and optional on transaction lookup. Must never be\n    placed in browser/client code.\n  required_on:\n  - POST /epay/api/v1/epay\n  - PUT /epay/api/v1/epay/cancel/{purchaseId}\n  - PUT /epay/api/v1/epay/changeAmount/{purchaseId}\n  - POST /onboarding/api/v1/location\n  - GET /onboarding/api/v1/location/{location}\n\
  \  - POST /developers-portal-service/api/v2/auth/login-link\n  - POST /alliance/api/v1/merchant-authentication\n  - GET /reports/api/v1/summary\n  - GET /reports/api/v1/detailed\n  - GET /reports/api/v1/customer-offer-history\n  optional_on:\n  - GET /epay/api/v1/epay\n  not_required_on:\n  - PUT /purchase/api/v1/online-link\n  - PUT /purchase/api/v1/payment-estimation\n  - POST /epay/api/v1/epay/send-link\n  sources:\n  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk\n  - https://docs.sunbit.com/docs/onboarding/adding-new-location\n- name: merchantAuthToken\n  type: http\n  scheme: bearer\n  description: >-\n    Short-lived bearer token minted by POST /alliance/api/v1/merchant-authentication for the\n    Payment Path SDK. Exchanged from sunbit-key + sunbit-secret plus a location; returned with\n    an ISO-8601 expiresAt. The docs instruct integrators to treat the token as opaque and not\n    parse it. Used browser-side to initialize the Payment Path module.\n  token_endpoint:\
  \ https://api.sunbit.com/alliance/api/v1/merchant-authentication\n  token_endpoint_sandbox: https://api-sandbox.sunbit.com/alliance/api/v1/merchant-authentication\n  expiry: ISO-8601 expiresAt returned with the token\n  sources:\n  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-payment-path\n- name: checkoutToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Per-transaction JWT returned by the checkout initialization call\n    (POST /epay/api/v1/epay). Handed to the browser and passed to SUNBIT.epay.checkout to\n    open the hosted checkout modal. Carries the retailer/alliance/transaction context and an\n    exp claim; it authorizes one checkout, not the API.\n  sources:\n  - https://docs.sunbit.com/docs/sdk-integrations/sunbit-checkout-sdk\nadditional_controls:\n- control: ip-allowlist\n  description: >-\n    Several endpoints are additionally restricted by source IP. The checkout initialization\n    call returns 403 \"IP address is not allowed for\
  \ this sunbitKey\" when the caller's IP does\n    not match the account, and the Customer Offer History report requires the requesting IP to\n    be on an authorized IP list (\"Your IP address is not registered to access this endpoint\").\n  applies_to:\n  - POST /epay/api/v1/epay\n  - GET /reports/api/v1/customer-offer-history\n  sources:\n  - https://docs.sunbit.com/docs/reporting/customer-offer-history-report\n- control: webhook-signature\n  description: >-\n    Inbound webhooks are authenticated to the integrator with an HMAC-SHA256 signature in the\n    Sunbit-Signature header (t=<unix-seconds>,v1=<hex>), signed over \"<timestamp>.<raw body>\"\n    with a per-endpoint secret generated in the developer portal. See asyncapi/sunbit-webhooks.yml.\n  sources:\n  - https://docs.sunbit.com/docs/webhooks/webhooks-verify-signature\ncredential_management:\n  issuance: >-\n    Credentials are not self-serve. Sunbit grants a partner access to the Sunbit Developers\n    Portal (developers.sunbit.com);\
  \ an administrator registers, then invites additional users\n    and manages their permissions. API keys for both sandbox and production are retrieved from\n    the portal's Keys tab.\n  production_access: >-\n    Production keys are gated behind a \"Request Production Access\" button in the portal, which\n    triggers Sunbit-side verification; the team is emailed when production is enabled.\n  portal: https://developers.sunbit.com/\n  sources:\n  - https://docs.sunbit.com/docs/overview/getting-started\n  - https://docs.sunbit.com/docs/overview/production-access\nobservations:\n- no OAuth 2.0 authorization server, no OpenID Connect discovery, and no published scopes\n- no /.well-known/oauth-authorization-server or /.well-known/openid-configuration on any host\n- secrets are long-lived shared credentials with no documented rotation or expiry policy\n- there is no documented mechanism for scoping a credential to a subset of operations\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunbit/refs/heads/main/authentication/sunbit-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Buy Now Pay Later
- point-of-sale-financing
- Consumer Lending
- Payments
- Fintech
- Checkout
- Merchant Onboarding
- Webhook
- Automotive
- Dental
- Veterinary
- Eyewear
- Healthcare Financing
- Embedded Finance
---
