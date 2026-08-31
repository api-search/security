---
api_key_in:
- header
api_specs:
- filename: cash-app-add-cash-app-pay-to-your-site-api-openapi.yml
  format: yaml
  label: Cash App Add Cash App Pay To Your Site API
  slug: cash-app-add-cash-app-pay-to-your-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-add-cash-app-pay-to-your-site-api-openapi.yml
- filename: cash-app-apikeys-api-openapi.yml
  format: yaml
  label: Cash App API Keys API
  slug: cash-app-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-apikeys-api-openapi.yml
- filename: cash-app-balances-api-openapi.yml
  format: yaml
  label: Cash App Balances API
  slug: cash-app-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-balances-api-openapi.yml
- filename: cash-app-billing-agreements-deprecated-api-openapi.yml
  format: yaml
  label: Cash App Billing Agreements (Deprecated) API
  slug: cash-app-billing-agreements-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-billing-agreements-deprecated-api-openapi.yml
- filename: cash-app-brands-api-openapi.yml
  format: yaml
  label: Cash App Brands API
  slug: cash-app-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-brands-api-openapi.yml
- filename: cash-app-customer-request-api-api-openapi.yml
  format: yaml
  label: Cash App Customer Request API
  slug: cash-app-customer-request-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-customer-request-api-api-openapi.yml
- filename: cash-app-customers-api-openapi.yml
  format: yaml
  label: Cash App Customers API
  slug: cash-app-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-customers-api-openapi.yml
- filename: cash-app-default-api-openapi.yml
  format: yaml
  label: Cash App App Default API
  slug: cash-app-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-default-api-openapi.yml
- filename: cash-app-disputes-api-openapi.yml
  format: yaml
  label: Cash App Disputes API
  slug: cash-app-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-disputes-api-openapi.yml
- filename: cash-app-feeplans-api-openapi.yml
  format: yaml
  label: Cash App Fee Plans API
  slug: cash-app-feeplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-feeplans-api-openapi.yml
- filename: cash-app-grants-afterpay-api-openapi.yml
  format: yaml
  label: Cash App Grants Afterpay API
  slug: cash-app-grants-afterpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-grants-afterpay-api-openapi.yml
- filename: cash-app-merchants-api-openapi.yml
  format: yaml
  label: Cash App Merchants API
  slug: cash-app-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-merchants-api-openapi.yml
- filename: cash-app-network-api-api-openapi.yml
  format: yaml
  label: Cash App Network API
  slug: cash-app-network-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-network-api-api-openapi.yml
- filename: cash-app-payments-api-openapi.yml
  format: yaml
  label: Cash App Payments API
  slug: cash-app-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-payments-api-openapi.yml
- filename: cash-app-payouts-api-openapi.yml
  format: yaml
  label: Cash App Payouts API
  slug: cash-app-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-payouts-api-openapi.yml
- filename: cash-app-refunds-api-openapi.yml
  format: yaml
  label: Cash App Refunds API
  slug: cash-app-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-refunds-api-openapi.yml
- filename: cash-app-requestchains-api-openapi.yml
  format: yaml
  label: Cash App Request Chains API
  slug: cash-app-requestchains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-requestchains-api-openapi.yml
- filename: cash-app-requests-api-openapi.yml
  format: yaml
  label: Cash App Requests API
  slug: cash-app-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-requests-api-openapi.yml
- filename: cash-app-webhooks-api-openapi.yml
  format: yaml
  label: Cash App Webhooks API
  slug: cash-app-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Cash App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cash App secures its APIs with apiKey, http, and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cash App
provider_slug: cash-app
scheme_count: 2
schemes:
- applies_to:
  - Cash App Pay Network API (api.cash.app/network/v1)
  - Cash App Pay Management API (api.cash.app/management/v1)
  - Cash App Pay Customer Request API (api.cash.app/customer-request/v1)
  authorization_header: Client {CLIENT_ID} {KEY_ID}
  key_lifecycle:
    bootstrap: client_id + client_secret used once to mint the first API_KEYS_READ/WRITE key
    expiry_days: 30
    expiry_field: expires_at
    provisioning: automated via Management API create-api-key (scoped keys)
    rotation: recommended several days before expiry; multiple least-privilege keys advised
  name: cash-app-pay-signed-api-key
  notes: 'Not OAuth2. Cash App Pay uses signed, scoped API keys: the Authorization header carries the

    client ID and key ID, and Network/Management requests must also carry an HMAC-SHA256 X-Signature

    computed with the key''s secret. Scopes (PAYMENTS_READ, API_KEYS_WRITE, ...) are attached per key;

    see scopes/cash-app-scopes.yml.

    '
  sandbox:
    host: sandbox.api.cash.app
    signature_bypass: 'X-Signature: sandbox:skip-signature-check'
  signature:
    algorithm: HMAC-SHA256
    body_digest: hex(SHA256(body)) lowercased
    header: X-Signature
    required_on:
    - Network API
    - Management API
    signed_headers:
    - Accept
    - Authorization
    - Content-Type
    - Host
    signed_string: '{method}\n{path}\n{headers}\n{bodyDigest}'
    value_format: V1 {signature}
  type: apiKey+hmac
- applies_to:
  - Afterpay Global API (global-api.afterpay.com)
  credentials: merchantId (username) + secretKey (password)
  name: afterpay-basic
  note: 'Afterpay/Cash App Afterpay Global API uses HTTP Basic auth (declared as securityScheme sec0 in

    the harvested OpenAPI). All endpoints except /ping require it; failure returns 401 Unauthorized.

    Afterpay docs note two supported auth options; Basic is the primary documented method.

    '
  scheme: basic
  sources:
  - openapi/cash-app-payments-openapi.json
  - openapi/cash-app-checkouts-openapi.json
  - openapi/cash-app-disputes-openapi.json
  - openapi/cash-app-configuration-openapi.json
  - openapi/cash-app-orders-openapi.json
  - openapi/cash-app-grants-afterpay-openapi.json
  - openapi/cash-app-grants-cash-app-pay-openapi.json
  - openapi/cash-app-billing-agreements-deprecated-openapi.json
  spec: RFC 7617
  type: http
slug: cash-app-authentication
source_filename: cash-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: |\n  https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/using-api-keys\n  https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/signing-requests\n  https://developers.cash.app/afterpay/api-reference/reference/introduction/authentication\ndocs:\n- https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/using-api-keys\n- https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/signing-requests\n- https://developers.cash.app/afterpay/api-reference/reference/introduction/authentication\nsummary:\n  types: [apiKey, http, hmac-signature]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: cash-app-pay-signed-api-key\n  applies_to:\n  - Cash App Pay Network API (api.cash.app/network/v1)\n  - Cash App Pay Management API (api.cash.app/management/v1)\n\
  \  - Cash App Pay Customer Request API (api.cash.app/customer-request/v1)\n  type: apiKey+hmac\n  authorization_header: 'Client {CLIENT_ID} {KEY_ID}'\n  signature:\n    header: X-Signature\n    value_format: 'V1 {signature}'\n    algorithm: HMAC-SHA256\n    signed_string: '{method}\\n{path}\\n{headers}\\n{bodyDigest}'\n    signed_headers: [Accept, Authorization, Content-Type, Host]\n    body_digest: hex(SHA256(body)) lowercased\n    required_on: [Network API, Management API]\n  key_lifecycle:\n    provisioning: automated via Management API create-api-key (scoped keys)\n    bootstrap: client_id + client_secret used once to mint the first API_KEYS_READ/WRITE key\n    expiry_days: 30\n    expiry_field: expires_at\n    rotation: recommended several days before expiry; multiple least-privilege keys advised\n  sandbox:\n    host: sandbox.api.cash.app\n    signature_bypass: 'X-Signature: sandbox:skip-signature-check'\n  notes: |\n    Not OAuth2. Cash App Pay uses signed, scoped API keys: the\
  \ Authorization header carries the\n    client ID and key ID, and Network/Management requests must also carry an HMAC-SHA256 X-Signature\n    computed with the key's secret. Scopes (PAYMENTS_READ, API_KEYS_WRITE, ...) are attached per key;\n    see scopes/cash-app-scopes.yml.\n- name: afterpay-basic\n  applies_to:\n  - Afterpay Global API (global-api.afterpay.com)\n  type: http\n  scheme: basic\n  spec: RFC 7617\n  credentials: merchantId (username) + secretKey (password)\n  sources:\n  - openapi/cash-app-payments-openapi.json\n  - openapi/cash-app-checkouts-openapi.json\n  - openapi/cash-app-disputes-openapi.json\n  - openapi/cash-app-configuration-openapi.json\n  - openapi/cash-app-orders-openapi.json\n  - openapi/cash-app-grants-afterpay-openapi.json\n  - openapi/cash-app-grants-cash-app-pay-openapi.json\n  - openapi/cash-app-billing-agreements-deprecated-openapi.json\n  note: |\n    Afterpay/Cash App Afterpay Global API uses HTTP Basic auth (declared as securityScheme sec0 in\n   \
  \ the harvested OpenAPI). All endpoints except /ping require it; failure returns 401 Unauthorized.\n    Afterpay docs note two supported auth options; Basic is the primary documented method.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/authentication/cash-app-authentication.yml
summary_line: apiKey/http/hmac-signature · 2 schemes
tags:
- Financial-Services
- Payments
- United States
- Fintech
- Neobank
- Buy Now Pay Later
- Payment Acceptance
- Digital Wallet
---
