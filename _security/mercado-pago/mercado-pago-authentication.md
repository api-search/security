---
api_key_in: []
api_specs:
- filename: mercado-pago-openapi.yml
  format: yaml
  label: Mercado Pago Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-openapi.yml
- filename: mercado-pago-asyncapi.yml
  format: yaml
  label: Mercado Pago Webhooks / Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/asyncapi/mercado-pago-asyncapi.yml
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
- Subscriptions
- POS
- QR
- PIX
- SDKs
- Wallet
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
