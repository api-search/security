---
api_key_in:
- body
- header
auth_types:
- apiKey
- http-bearer-jwt
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Coda Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coda Payments secures its APIs with apiKey, http-bearer-jwt, and hmac-signature across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coda Payments
provider_slug: coda-payments
scheme_count: 9
schemes:
- api: Codapay Hosted Payment Page API
  description: API key issued by Coda in the Publisher Portal and passed inside the JSON request body. In v1.0 one key is issued per title-country combination; in v2.0 a single global API key per merchant is used together with a mandatory projectId field.
  in: body
  name: codapay-api-key
  parameter: initRequest.apiKey
  source: https://docs.coda.co/codapay/integration-guides/codapay-api-versions.md
  type: apiKey
- api: Codapay Hosted Payment Page API
  description: Project ID issued per title product; mandatory on all v2.0 requests.
  in: body
  name: codapay-project-id
  parameter: initRequest.projectId
  required_for: v2.0
  source: https://docs.coda.co/codapay/integration-guides/codapay-api-versions.md
  type: apiKey
- api: Codapay Direct Card API
  description: '"Include an Authorization header, API Key, and Partner ID" — the Direct Card API (submit a charge, get charge data, calculate tax, create refund) is authenticated with a partner id plus a secret API key, over TLS 1.2 or higher.'
  in: header
  name: direct-card-api-headers
  parameters:
  - Authorization
  - X-Api-Key
  - X-Partner-Id
  source: https://docs.coda.co/codapay/direct-api-integration/direct-api-integration-for-cards/submit-a-charge.md
  type: apiKey
- api: Coda Payout API
  bearerFormat: JWT
  description: JWT generated per request and sent as "Bearer {jwt}". Accompanied by X-API-Key and an x-signature integrity checksum header; Content-Type must be application/json.
  header: Authorization
  name: payout-jwt
  scheme: bearer
  source: https://docs.coda.co/payout/integration-guides/getting-started/how-to-generate-the-jwt-token.md
  type: http
- api: Coda Payout API
  description: Merchant API key required on every Payout API request.
  in: header
  name: payout-api-key
  parameter: X-API-Key
  source: https://docs.coda.co/payout/integration-guides/getting-started/authentication-and-authorization.md
  type: apiKey
- api: Coda Payout API
  description: Request-integrity checksum computed over the payload; required on every request.
  in: header
  name: payout-x-signature
  parameter: x-signature
  source: https://docs.coda.co/payout/integration-guides/getting-started/how-to-generate-the-x-signature.md
  type: hmac-signature
- api: Codapay Tokenization API 2.0 (archived)
  bearerFormat: JWT
  description: HS256 JWT signed with a partner JWT secret, unique per request, plus X-Partner-Id (the "username") and X-Api-Key (the secret). Documented under the archived Tokenization API 2.0 section.
  headers:
  - Authorization
  - X-Partner-Id
  - X-Api-Key
  jwt_algorithm: HS256
  jwt_claims:
  - partner_id
  - iat
  name: tokenization-jwt
  scheme: bearer
  source: https://docs.coda.co/codapay/archived-tokenization-api-2.0/security-and-authentication.md
  type: http
- algorithm: HMAC-SHA256
  api: Codashop and Coda Webstore Fulfillment API
  description: Publisher-side fulfillment endpoints (validate, topup, usersync) authenticate Coda's calls with an HMAC-SHA256 signature over an ordered concatenation of request fields (id + jsonrpc + method + serviceProvider + txnId + orderId + userId + zoneId + currency + amount + sku + quantity + paymentChannelId + isForTest [+ roleId]) using a merchant-defined shared secret key.
  in: body
  name: codashop-fulfillment-hmac
  parameter: signature
  source: https://docs.coda.co/codashop-and-distribution/integration-guides/authorization.md
  type: hmac-signature
- algorithm: MD5
  api: Codapay Hosted Payment Page API
  description: Transaction completion notifications carry a Checksum query parameter that partners must validate before processing. Payin formula is MD5(txnId + apiKey + orderId + resultCode); separate formulas are published for save-card and refund/chargeback notifications.
  direction: inbound-webhook
  in: query
  name: notification-checksum
  parameter: Checksum
  source: https://docs.coda.co/codapay/integration-guides/security-guidelines.md
  type: hmac-signature
slug: coda-payments-authentication
source_filename: coda-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.coda.co/\ndocs:\n- https://docs.coda.co/codapay/getting-started/set-up-payments.md\n- https://docs.coda.co/payout/integration-guides/getting-started/authentication-and-authorization.md\n- https://docs.coda.co/codashop-and-distribution/integration-guides/authorization.md\n- https://docs.coda.co/codapay/archived-tokenization-api-2.0/security-and-authentication.md\nnote: >-\n  Coda Payments publishes no OpenAPI/Swagger definition for any of its APIs, so this\n  profile was read from the published documentation rather than derived from a spec.\n  Every surface below was confirmed on docs.coda.co on 2026-08-04.\nsummary:\n  types:\n  - apiKey\n  - http-bearer-jwt\n  - hmac-signature\n  api_key_in:\n  - body\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  transport_requirements:\n  - HTTPS only\n  - TLS 1.2 or higher\nschemes:\n- name: codapay-api-key\n  api: Codapay\
  \ Hosted Payment Page API\n  type: apiKey\n  in: body\n  parameter: initRequest.apiKey\n  description: >-\n    API key issued by Coda in the Publisher Portal and passed inside the JSON request\n    body. In v1.0 one key is issued per title-country combination; in v2.0 a single\n    global API key per merchant is used together with a mandatory projectId field.\n  source: https://docs.coda.co/codapay/integration-guides/codapay-api-versions.md\n- name: codapay-project-id\n  api: Codapay Hosted Payment Page API\n  type: apiKey\n  in: body\n  parameter: initRequest.projectId\n  required_for: v2.0\n  description: Project ID issued per title product; mandatory on all v2.0 requests.\n  source: https://docs.coda.co/codapay/integration-guides/codapay-api-versions.md\n- name: direct-card-api-headers\n  api: Codapay Direct Card API\n  type: apiKey\n  in: header\n  parameters:\n  - Authorization\n  - X-Api-Key\n  - X-Partner-Id\n  description: >-\n    \"Include an Authorization header, API Key, and\
  \ Partner ID\" — the Direct Card API\n    (submit a charge, get charge data, calculate tax, create refund) is authenticated\n    with a partner id plus a secret API key, over TLS 1.2 or higher.\n  source: https://docs.coda.co/codapay/direct-api-integration/direct-api-integration-for-cards/submit-a-charge.md\n- name: payout-jwt\n  api: Coda Payout API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: Authorization\n  description: >-\n    JWT generated per request and sent as \"Bearer {jwt}\". Accompanied by X-API-Key\n    and an x-signature integrity checksum header; Content-Type must be application/json.\n  source: https://docs.coda.co/payout/integration-guides/getting-started/how-to-generate-the-jwt-token.md\n- name: payout-api-key\n  api: Coda Payout API\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Merchant API key required on every Payout API request.\n  source: https://docs.coda.co/payout/integration-guides/getting-started/authentication-and-authorization.md\n\
  - name: payout-x-signature\n  api: Coda Payout API\n  type: hmac-signature\n  in: header\n  parameter: x-signature\n  description: Request-integrity checksum computed over the payload; required on every request.\n  source: https://docs.coda.co/payout/integration-guides/getting-started/how-to-generate-the-x-signature.md\n- name: tokenization-jwt\n  api: Codapay Tokenization API 2.0 (archived)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  headers:\n  - Authorization\n  - X-Partner-Id\n  - X-Api-Key\n  jwt_algorithm: HS256\n  jwt_claims:\n  - partner_id\n  - iat\n  description: >-\n    HS256 JWT signed with a partner JWT secret, unique per request, plus X-Partner-Id\n    (the \"username\") and X-Api-Key (the secret). Documented under the archived\n    Tokenization API 2.0 section.\n  source: https://docs.coda.co/codapay/archived-tokenization-api-2.0/security-and-authentication.md\n- name: codashop-fulfillment-hmac\n  api: Codashop and Coda Webstore Fulfillment API\n  type: hmac-signature\n\
  \  algorithm: HMAC-SHA256\n  parameter: signature\n  in: body\n  description: >-\n    Publisher-side fulfillment endpoints (validate, topup, usersync) authenticate Coda's\n    calls with an HMAC-SHA256 signature over an ordered concatenation of request fields\n    (id + jsonrpc + method + serviceProvider + txnId + orderId + userId + zoneId +\n    currency + amount + sku + quantity + paymentChannelId + isForTest [+ roleId]) using\n    a merchant-defined shared secret key.\n  source: https://docs.coda.co/codashop-and-distribution/integration-guides/authorization.md\n- name: notification-checksum\n  api: Codapay Hosted Payment Page API\n  type: hmac-signature\n  algorithm: MD5\n  parameter: Checksum\n  in: query\n  direction: inbound-webhook\n  description: >-\n    Transaction completion notifications carry a Checksum query parameter that partners\n    must validate before processing. Payin formula is MD5(txnId + apiKey + orderId +\n    resultCode); separate formulas are published for save-card\
  \ and refund/chargeback\n    notifications.\n  source: https://docs.coda.co/codapay/integration-guides/security-guidelines.md\nip_allowlisting:\n  supported: true\n  description: >-\n    Coda publishes IP allowlist requirements for the Direct Card API and for Codashop\n    fulfillment callbacks; partners must whitelist Coda's egress addresses.\n  sources:\n  - https://docs.coda.co/codapay/direct-api-integration/direct-api-integration-for-cards/whitelist-ip-address.md\n  - https://docs.coda.co/changelog/2024-codashop-changelog/codashop-ip-whitelist-changes.md\ncredential_issuance:\n  portal: https://portal.coda.co/\n  description: >-\n    API keys, project ids and sandbox/production configuration are issued and rotated\n    in the Coda Publisher Portal; there is no self-service public signup for API\n    credentials beyond portal registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda-payments/refs/heads/main/authentication/coda-payments-authentication.yml
summary_line: apiKey/http-bearer-jwt/hmac-signature · 9 schemes
tags:
- Company
- Payments
- Merchant of Record
- Gaming
- Digital Goods
- Carrier Billing
- E-Wallets
- Payouts
- Southeast Asia
- Monetization
---
