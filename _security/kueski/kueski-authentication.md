---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kueski Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kueski secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kueski
provider_slug: kueski
scheme_count: 2
schemes:
- audience: browser / client-side
  distribution: The public key is passed to the CDN widget loader as a query parameter — https://cdn.kueskipay.com/widgets.js?authorization={public_key}&integration={platform}&version={v}&sandbox={true|false} — and the widget then replays it as an Authorization bearer token against the configuration API. It is a publishable key by design and is visible in merchant page source.
  format: 'Authorization: Bearer {merchant_public_key}'
  in: header
  name: merchantPublicKeyBearer
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://cdn.kueskipay.com/widgets.js
  type: http
  used_by:
  - api: Kueski Pay Widget Configuration API
    host: https://api.kueskipay.com
    operations:
    - GET /v1/configurations?widget_type=product_widget
    sandbox_host: https://testing.kueskipay.com
- audience: server-to-server
  format: 'Authorization: Bearer {merchant_api_key}'
  in: header
  name: merchantApiKeyBearer
  notes: The key-validation operation is the exception to the bearer pattern — validate-keys accepts the merchant API key as an api_key query-string parameter rather than an Authorization header. All other merchant operations use the bearer header. Transporting a credential in the query string means it can be captured in intermediary access logs; this is a design weakness worth raising with Kueski.
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://wordpress.org/plugins/kueskipay-gateway/
  type: http
  used_by:
  - api: Kueski Pay Merchant Orders API
    host: https://woocommerce-middleware-go.production-pay.kueski.com/api/v1
    operations:
    - GET /api/v1/merchant/validate-keys?api_key={merchant_api_key}
    - POST /api/v1/order/create
    - POST /api/v1/orders-sync
    - POST /api/v1/order/refund
    sandbox_host: https://woocommerce-middleware-go.staging-pay.kueski.codes/api/v1
slug: kueski-authentication
source_filename: kueski-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: >-\n  Derived from Kueski first-party published sources: the widgets.js bundle at\n  https://cdn.kueskipay.com/widgets.js and the KueskiPay Gateway WooCommerce plugin v2.4.1\n  (Author: Kueski) at https://wordpress.org/plugins/kueskipay-gateway/ ; confirmed against a live\n  unauthenticated probe of https://api.kueskipay.com/v1/configurations\ndocs: https://github.com/kueski-dev/Dev-Center/wiki\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Kueski Pay authenticates with opaque merchant API keys presented as HTTP bearer tokens. There is\n    no OAuth 2.0, no OpenID Connect, and no scope surface — so no scopes/ artifact is emitted for\n    this provider. Merchants are issued a public key (safe for browser use, drives the widgets) and\n    a secret/private API key (server-side, drives order creation, sync and refunds).\
  \ Both are\n    provisioned by Kueski to the merchant out of band via the merchant portal at\n    https://negocios.kueski.com/login — there is no self-service key-generation API.\nschemes:\n- name: merchantPublicKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: 'Authorization: Bearer {merchant_public_key}'\n  audience: browser / client-side\n  used_by:\n  - api: Kueski Pay Widget Configuration API\n    host: https://api.kueskipay.com\n    sandbox_host: https://testing.kueskipay.com\n    operations:\n    - 'GET /v1/configurations?widget_type=product_widget'\n  distribution: >-\n    The public key is passed to the CDN widget loader as a query parameter —\n    https://cdn.kueskipay.com/widgets.js?authorization={public_key}&integration={platform}&version={v}&sandbox={true|false}\n    — and the widget then replays it as an Authorization bearer token against the configuration API.\n    It is a publishable key by design and is visible in merchant\
  \ page source.\n  sources:\n  - https://cdn.kueskipay.com/widgets.js\n- name: merchantApiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: 'Authorization: Bearer {merchant_api_key}'\n  audience: server-to-server\n  used_by:\n  - api: Kueski Pay Merchant Orders API\n    host: https://woocommerce-middleware-go.production-pay.kueski.com/api/v1\n    sandbox_host: https://woocommerce-middleware-go.staging-pay.kueski.codes/api/v1\n    operations:\n    - 'GET /api/v1/merchant/validate-keys?api_key={merchant_api_key}'\n    - 'POST /api/v1/order/create'\n    - 'POST /api/v1/orders-sync'\n    - 'POST /api/v1/order/refund'\n  notes: >-\n    The key-validation operation is the exception to the bearer pattern — validate-keys accepts the\n    merchant API key as an api_key query-string parameter rather than an Authorization header. All\n    other merchant operations use the bearer header. Transporting a credential in the query string\n    means it can\
  \ be captured in intermediary access logs; this is a design weakness worth raising\n    with Kueski.\n  sources:\n  - https://wordpress.org/plugins/kueskipay-gateway/\nkey_management:\n  self_service: false\n  rotation_documented: false\n  expiry_documented: false\n  provisioning: >-\n    Keys (\"API Publica\" and \"API Secreta\") are supplied to the merchant by Kueski after merchant\n    onboarding at https://www.kueskipay.com/registro-comercios and are entered into the platform\n    plugin's settings screen. No public documentation describes key rotation, revocation or expiry.\nobserved_failures:\n- condition: no Authorization header\n  http_status: 400\n  body: '{\"status\":\"fail\",\"code\":\"unauthorized\",\"message\":\"no token provided\"}'\n- condition: malformed or unknown bearer token\n  http_status: 400\n  body: '{\"status\":\"fail\",\"code\":\"unauthorized\",\"message\":\"invalid token provided\"}'\n- note: >-\n    Both authentication failures are returned as HTTP 400 Bad Request\
  \ rather than 401 Unauthorized,\n    and neither emits a WWW-Authenticate challenge header. This is a real conformance deviation from\n    RFC 9110 section 15.5.2 and is recorded in conformance/kueski-conformance.yml.\ngaps:\n- No published authentication reference page; the auth model has to be reconstructed from\n  first-party plugin source and the widget bundle.\n- No OAuth 2.0 / OIDC surface, so no delegated access and no scoped, least-privilege credentials\n  for third-party or agent integrations.\n- No documented key rotation or revocation procedure.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - {url: 'https://api.kueskipay.com/v1/configurations?widget_type=product_widget', http_status: 400, content_type: application/json}\n  - {url: 'https://cdn.kueskipay.com/widgets.js', http_status: 200, content_type: application/javascript}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kueski/refs/heads/main/authentication/kueski-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Payments
- Buy Now Pay Later
- Lending
- Fintech
- Financial-Services
- Consumer Credit
- E-Commerce
- Checkout
- Mexico
- Latin America
---
