---
api_key_in:
- header
api_specs:
- filename: shopback-account-linking-api-openapi.yml
  format: yaml
  label: ShopBack Account Linking API
  slug: shopback-account-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-account-linking-api-openapi.yml
- filename: shopback-authentication-api-openapi.yml
  format: yaml
  label: ShopBack Authentication API
  slug: shopback-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-authentication-api-openapi.yml
- filename: shopback-notification-api-openapi.yml
  format: yaml
  label: ShopBack Notification API
  slug: shopback-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-notification-api-openapi.yml
- filename: shopback-orders-api-openapi.yml
  format: yaml
  label: ShopBack Orders API
  slug: shopback-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-orders-api-openapi.yml
- filename: shopback-pre-auth-api-openapi.yml
  format: yaml
  label: ShopBack Pre Auth API
  slug: shopback-pre-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-pre-auth-api-openapi.yml
auth_types:
- http
- hmac
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shopback Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShopBack secures its APIs with http, hmac, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShopBack
provider_slug: shopback
scheme_count: 3
schemes:
- api: ShopBack Online Payments API
  bearerFormat: JWT
  credentials:
    docs: https://docs.shopback.com/docs/online-payment-credentials
    issued_by: ShopBack for Business merchant portal, Settings → Generate credential
    note: The Merchant Secret can only be viewed once, at generation time.
    password: Merchant Secret (separate sandbox and production values)
    portals:
    - https://business.shopback.sg/signin
    - https://business.shopback.my/signin
    username: Merchant ID
  description: Merchant JWT obtained from the merchant login operation.
  guidance: ShopBack recommends generating a new token per transaction.
  header: 'Authorization: Bearer <merchant_jwt>'
  name: bearer
  scheme: bearer
  sources:
  - openapi/shopback-online-payments-openapi.yml
  - https://docs.shopback.com/docs/token-validity
  token_endpoint: POST /auth/login
  token_endpoint_note: The published securityScheme description says "POST /merchant-gateway/auth/login", while the documented path item (operationId `login`) is /auth/login relative to the declared server. Recorded verbatim; not reconciled.
  token_lifetime: 8 hours
  type: http
- additional_required_headers:
  - description: ISO-8601 UTC timestamp; must be byte-identical to the value used in the signature. Non-UTC offsets or roughly a minute of clock skew expire the signature.
    name: Date
  - description: application/json
    name: Content-Type
  algorithm: HMAC-SHA256
  api: ShopBack In-Store Payments API
  credentials:
    accessKeyId: identifier paired with the secret
    accessKeySecret: HMAC signing secret
    note: Sandbox and production credentials differ; production keys are issued at go-live.
    posId: one per terminal, kiosk, cashier register, app or website instance
  encoding: hex
  header: 'Authorization: SB1-HMAC-SHA256 <accessKeyId>:<hmacSignature>'
  name: SB1-HMAC-SHA256
  signed_string_order:
  - HTTP method (uppercase)
  - request content type
  - ISO-8601 UTC date-time
  - fully qualified request path including query parameters
  - SHA-256 hex digest of the alphabetically key-sorted, stringified JSON body
  sources:
  - https://docs.shopback.com/reference/generating-hmac-signature
  - https://docs.shopback.com/reference/in-store-getting-started
  - openapi/shopback-in-store-payments-openapi.yml
  type: hmac
- api: ShopBack Online Payments API (tokenized payments, client-side)
  description: Short-lived JWT returned by the link-session endpoint. Passed by the merchant app as a custom header when opening the ShopBack consent page in an in-app browser (SFSafariViewController / Chrome Custom Tabs). Not a server-to-server credential.
  in: header
  name: X-ShopBack-App-Token
  parameter_name: X-ShopBack-App-Token
  sources:
  - https://docs.shopback.com/reference/account-linking-1
  - openapi/shopback-online-payments-openapi.yml
  type: apiKey
slug: shopback-authentication
source_filename: shopback-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: >-\n  derived from openapi/shopback-online-payments-openapi.yml securitySchemes,\n  upgraded from https://docs.shopback.com/reference/getting-started-authentication,\n  https://docs.shopback.com/reference/generating-hmac-signature,\n  https://docs.shopback.com/docs/token-validity and\n  https://docs.shopback.com/docs/online-payment-credentials\ndocs: https://docs.shopback.com/reference/generating-hmac-signature\nsummary:\n  types: [http, hmac, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    ShopBack publishes two distinct auth models, one per API. Only the Online\n    Payments API declares a securityScheme in its OpenAPI; the In-Store Payments\n    API models its credentials as required header parameters rather than a\n    declared scheme, so the derived pass alone missed it.\nschemes:\n- name: bearer\n  api: ShopBack Online Payments API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description:\
  \ Merchant JWT obtained from the merchant login operation.\n  header: 'Authorization: Bearer <merchant_jwt>'\n  token_endpoint: POST /auth/login\n  token_endpoint_note: >-\n    The published securityScheme description says \"POST\n    /merchant-gateway/auth/login\", while the documented path item (operationId\n    `login`) is /auth/login relative to the declared server. Recorded verbatim;\n    not reconciled.\n  credentials:\n    username: Merchant ID\n    password: Merchant Secret (separate sandbox and production values)\n    issued_by: ShopBack for Business merchant portal, Settings → Generate credential\n    portals:\n    - https://business.shopback.sg/signin\n    - https://business.shopback.my/signin\n    docs: https://docs.shopback.com/docs/online-payment-credentials\n    note: The Merchant Secret can only be viewed once, at generation time.\n  token_lifetime: 8 hours\n  guidance: ShopBack recommends generating a new token per transaction.\n  sources:\n  - openapi/shopback-online-payments-openapi.yml\n\
  \  - https://docs.shopback.com/docs/token-validity\n- name: SB1-HMAC-SHA256\n  api: ShopBack In-Store Payments API\n  type: hmac\n  algorithm: HMAC-SHA256\n  encoding: hex\n  header: 'Authorization: SB1-HMAC-SHA256 <accessKeyId>:<hmacSignature>'\n  additional_required_headers:\n  - name: Date\n    description: ISO-8601 UTC timestamp; must be byte-identical to the value used\n      in the signature. Non-UTC offsets or roughly a minute of clock skew expire\n      the signature.\n  - name: Content-Type\n    description: application/json\n  signed_string_order:\n  - HTTP method (uppercase)\n  - request content type\n  - ISO-8601 UTC date-time\n  - fully qualified request path including query parameters\n  - SHA-256 hex digest of the alphabetically key-sorted, stringified JSON body\n  credentials:\n    accessKeyId: identifier paired with the secret\n    accessKeySecret: HMAC signing secret\n    posId: one per terminal, kiosk, cashier register, app or website instance\n    note: Sandbox and\
  \ production credentials differ; production keys are issued at\n      go-live.\n  sources:\n  - https://docs.shopback.com/reference/generating-hmac-signature\n  - https://docs.shopback.com/reference/in-store-getting-started\n  - openapi/shopback-in-store-payments-openapi.yml\n- name: X-ShopBack-App-Token\n  api: ShopBack Online Payments API (tokenized payments, client-side)\n  type: apiKey\n  in: header\n  parameter_name: X-ShopBack-App-Token\n  description: >-\n    Short-lived JWT returned by the link-session endpoint. Passed by the merchant\n    app as a custom header when opening the ShopBack consent page in an in-app\n    browser (SFSafariViewController / Chrome Custom Tabs). Not a server-to-server\n    credential.\n  sources:\n  - https://docs.shopback.com/reference/account-linking-1\n  - openapi/shopback-online-payments-openapi.yml\nbearer_tokens_of_record:\n- name: paymentToken\n  kind: long-lived user payment token\n  description: >-\n    Issued after a user completes the ShopBack\
  \ consent flow; scoped to one user\n    and one merchant channel. States LINKED / UNLINKED. Not an API credential —\n    it is a payment instrument reference sent in the request body.\n  docs: https://docs.shopback.com/reference/account-linking-1\noauth2:\n  supported: false\n  note: >-\n    Account linking is OAuth-shaped (hosted consent page, single-use 60-second\n    auth code, code-for-token exchange, revocation endpoint) but is not an OAuth\n    2.0 profile: there is no authorization-server metadata, no scope model, no\n    refresh token, and /.well-known/oauth-authorization-server returns 404 on\n    every ShopBack host. No scopes/ artifact was written for this reason.\ntransport:\n  https_required: true\n  tls_minimum: TLS 1.2\n  source: https://docs.shopback.com/docs/quickstart-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/authentication/shopback-authentication.yml
summary_line: http/hmac/apiKey · 3 schemes
tags:
- Company
- Payments
- Cashback
- Rewards
- Loyalty
- E-Commerce
- Buy Now Pay Later
- Point Of Sale
- Checkout
- Singapore
---
