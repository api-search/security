---
api_key_in: []
api_specs:
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Checkout API
  slug: yoco-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Refunds API
  slug: yoco-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Webhooks API
  slug: yoco-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payments API
  slug: yoco-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payment Links API
  slug: yoco-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Yoco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yoco secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yoco
provider_slug: yoco
scheme_count: 2
schemes:
- description: 'Secret integration key for the Checkout API (https://payments.yoco.com/api), passed as `Authorization: Bearer sk_live_...` (live) or `Authorization: Bearer sk_test_...` (test). Keys are self-served from the Yoco app under Sales -> Payment Gateway. The Checkout API must be called server-side so the secret key is never exposed to the browser.'
  name: secretKey
  scheme: bearer
  sources:
  - https://developer.yoco.com/online/resources/integration-keys/
  - https://developer.yoco.com/online/resources/get-started
  type: http
- bearerFormat: JWT
  description: JWT Bearer credential for the versioned Yoco API (https://api.yoco.com/v1, sandbox https://api.yocosandbox.com/v1), authorized with OAuth-style scopes such as business/orders:read. Used by the payments, refunds, and payment-links read endpoints.
  name: jwtBearer
  scheme: bearer
  sources:
  - https://developer.yoco.com/api-reference/yoco-api/payments/list-payments-v-1-payments-get
  - https://developer.yoco.com/api-reference/yoco-api/refunds/fetch-refund-v-1-refunds-refund-id-get
  type: http
slug: yoco-authentication
source_filename: yoco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: openapi/yoco-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: secretKey\n  type: http\n  scheme: bearer\n  description: >-\n    Secret integration key for the Checkout API (https://payments.yoco.com/api),\n    passed as `Authorization: Bearer sk_live_...` (live) or\n    `Authorization: Bearer sk_test_...` (test). Keys are self-served from the\n    Yoco app under Sales -> Payment Gateway. The Checkout API must be called\n    server-side so the secret key is never exposed to the browser.\n  sources:\n  - https://developer.yoco.com/online/resources/integration-keys/\n  - https://developer.yoco.com/online/resources/get-started\n- name: jwtBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    JWT Bearer credential for the versioned Yoco API\n    (https://api.yoco.com/v1, sandbox https://api.yocosandbox.com/v1),\n    authorized with OAuth-style scopes such as business/orders:read. Used\
  \ by\n    the payments, refunds, and payment-links read endpoints.\n  sources:\n  - https://developer.yoco.com/api-reference/yoco-api/payments/list-payments-v-1-payments-get\n  - https://developer.yoco.com/api-reference/yoco-api/refunds/fetch-refund-v-1-refunds-refund-id-get\nwebhookVerification:\n  description: >-\n    Outbound webhook deliveries are signed. Each request carries webhook-id,\n    webhook-timestamp, and webhook-signature headers. Verify by computing an\n    HMAC-SHA256 over the signed content (id.timestamp.payload) with your\n    endpoint's signing secret, base64-encoding the result, and comparing in\n    constant time. Reject deliveries whose webhook-timestamp is outside an\n    acceptable threshold (Yoco recommends ~3 minutes).\n  sources:\n  - https://developer.yoco.com/online/api-reference/webhooks/verifying-events/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/authentication/yoco-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Fintech
- Payment Gateway
- Card Payments
- South Africa
- Online Payments
- Checkout
- Point of Sale
- SMB
- Financial Infrastructure
---
