---
api_key_in: []
api_specs:
- filename: mercado-pago-asyncapi.yml
  format: yaml
  label: Mercado Pago Webhooks / Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/asyncapi/mercado-pago-asyncapi.yml
- filename: mercado-pago-authentication-api-openapi.yml
  format: yaml
  label: Mercado Pago Authentication API
  slug: mercado-pago-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-authentication-api-openapi.yml
- filename: mercado-pago-cards-api-openapi.yml
  format: yaml
  label: Mercado Pago Cards API
  slug: mercado-pago-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-cards-api-openapi.yml
- filename: mercado-pago-chargebacks-api-openapi.yml
  format: yaml
  label: Mercado Pago Chargebacks API
  slug: mercado-pago-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-chargebacks-api-openapi.yml
- filename: mercado-pago-claims-api-openapi.yml
  format: yaml
  label: Mercado Pago Claims API
  slug: mercado-pago-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-claims-api-openapi.yml
- filename: mercado-pago-customers-api-openapi.yml
  format: yaml
  label: Mercado Pago Customers API
  slug: mercado-pago-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-customers-api-openapi.yml
- filename: mercado-pago-merchant-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Merchant Orders API
  slug: mercado-pago-merchant-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-merchant-orders-api-openapi.yml
- filename: mercado-pago-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Orders API
  slug: mercado-pago-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-orders-api-openapi.yml
- filename: mercado-pago-payment-methods-api-openapi.yml
  format: yaml
  label: Mercado Pago Payment Methods API
  slug: mercado-pago-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payment-methods-api-openapi.yml
- filename: mercado-pago-payments-api-openapi.yml
  format: yaml
  label: Mercado Pago Payments API
  slug: mercado-pago-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payments-api-openapi.yml
- filename: mercado-pago-plans-api-openapi.yml
  format: yaml
  label: Mercado Pago Plans API
  slug: mercado-pago-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-plans-api-openapi.yml
- filename: mercado-pago-point-api-openapi.yml
  format: yaml
  label: Mercado Pago Point API
  slug: mercado-pago-point-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-point-api-openapi.yml
- filename: mercado-pago-preferences-api-openapi.yml
  format: yaml
  label: Mercado Pago Preferences API
  slug: mercado-pago-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-preferences-api-openapi.yml
- filename: mercado-pago-qr-api-openapi.yml
  format: yaml
  label: Mercado Pago QR API
  slug: mercado-pago-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-qr-api-openapi.yml
- filename: mercado-pago-refunds-api-openapi.yml
  format: yaml
  label: Mercado Pago Refunds API
  slug: mercado-pago-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-refunds-api-openapi.yml
- filename: mercado-pago-reports-api-openapi.yml
  format: yaml
  label: Mercado Pago Reports API
  slug: mercado-pago-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-reports-api-openapi.yml
- filename: mercado-pago-subscriptions-api-openapi.yml
  format: yaml
  label: Mercado Pago Subscriptions API
  slug: mercado-pago-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-subscriptions-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mercado Pago Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mercado Pago secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mercado Pago
provider_slug: mercado-pago
scheme_count: 2
schemes:
- bearerFormat: access_token
  description: 'Mercado Pago access token. Send as `Authorization: Bearer {ACCESS_TOKEN}`.

    HTTPS is required. Idempotency is supported via the `X-Idempotency-Key`

    header on POST/PUT operations.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mercado-pago-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://auth.mercadopago.com/authorization
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.mercadopago.com/oauth/token
  name: oauth2
  sources:
  - openapi/mercado-pago-openapi.yml
  type: oauth2
slug: mercado-pago-authentication
source_filename: mercado-pago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mercado-pago-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  description: |-\n    Mercado Pago access token. Send as `Authorization: Bearer {ACCESS_TOKEN}`.\n    HTTPS is required. Idempotency is supported via the `X-Idempotency-Key`\n    header on POST/PUT operations.\n  sources:\n  - openapi/mercado-pago-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mercadopago.com/authorization\n    tokenUrl: https://api.mercadopago.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/mercado-pago-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/authentication/mercado-pago-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- Checkout
- Subscription
- Point-of-Sale
- QR
- Pix
- SDK
- Wallets
- Acquiring
- Lending
- Issuing
- Latin America
- Brazil
- Argentina
- Mexico
- Chile
- Colombia
- Peru
- Uruguay
- Fintech
---
