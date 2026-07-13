---
api_key_in: []
api_specs:
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Payments API
  slug: moyasar-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Invoices API
  slug: moyasar-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Tokens API
  slug: moyasar-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Webhooks API
  slug: moyasar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Payouts API
  slug: moyasar-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moyasar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moyasar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moyasar
provider_slug: moyasar
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The API key is passed as the username and the password is left empty (e.g. `curl https://api.moyasar.com/v1/payments -u sk_test_123:`). All requests must be over HTTPS. Publishable keys (pk_test_ / pk_live_) are safe for client-side use and may only create payments and tokens; secret keys (sk_test_ / sk_live_) authorize all account operations and must remain on the backend. Test-mode keys drive a sandbox, live-mode keys move real money.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/moyasar-openapi.yml
  - https://docs.moyasar.com/api/authentication
  type: http
slug: moyasar-authentication
source_filename: moyasar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/moyasar-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The API key is passed as the username and the\n    password is left empty (e.g. `curl https://api.moyasar.com/v1/payments -u\n    sk_test_123:`). All requests must be over HTTPS. Publishable keys\n    (pk_test_ / pk_live_) are safe for client-side use and may only create\n    payments and tokens; secret keys (sk_test_ / sk_live_) authorize all account\n    operations and must remain on the backend. Test-mode keys drive a sandbox,\n    live-mode keys move real money.\n  sources:\n  - openapi/moyasar-openapi.yml\n  - https://docs.moyasar.com/api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/authentication/moyasar-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Saudi Arabia
- MENA
- mada
- Cards
- Apple Pay
- STC Pay
- Invoices
- Fintech
---
