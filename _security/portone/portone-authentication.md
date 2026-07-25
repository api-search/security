---
api_key_in: []
api_specs:
- filename: portone-b2b-api-openapi.yml
  format: yaml
  label: PortOne B2b API
  slug: portone-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-b2b-api-openapi.yml
- filename: portone-banks-api-openapi.yml
  format: yaml
  label: PortOne Banks API
  slug: portone-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-banks-api-openapi.yml
- filename: portone-billing-keys-api-openapi.yml
  format: yaml
  label: PortOne Billing Keys API
  slug: portone-billing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-billing-keys-api-openapi.yml
- filename: portone-cash-receipts-api-openapi.yml
  format: yaml
  label: PortOne Cash Receipts API
  slug: portone-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-cash-receipts-api-openapi.yml
- filename: portone-checkout-profiles-api-openapi.yml
  format: yaml
  label: PortOne Checkout Profiles API
  slug: portone-checkout-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-checkout-profiles-api-openapi.yml
- filename: portone-identity-verifications-api-openapi.yml
  format: yaml
  label: PortOne Identity Verifications API
  slug: portone-identity-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-identity-verifications-api-openapi.yml
- filename: portone-kakaopay-api-openapi.yml
  format: yaml
  label: PortOne Kakaopay API
  slug: portone-kakaopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-kakaopay-api-openapi.yml
- filename: portone-login-api-openapi.yml
  format: yaml
  label: PortOne Login API
  slug: portone-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-login-api-openapi.yml
- filename: portone-payment-events-by-cursor-api-openapi.yml
  format: yaml
  label: PortOne Payment Events By Cursor API
  slug: portone-payment-events-by-cursor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-events-by-cursor-api-openapi.yml
- filename: portone-payment-gateways-api-openapi.yml
  format: yaml
  label: PortOne Payment Gateways API
  slug: portone-payment-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-gateways-api-openapi.yml
- filename: portone-payment-reconciliations-api-openapi.yml
  format: yaml
  label: PortOne Payment Reconciliations API
  slug: portone-payment-reconciliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-reconciliations-api-openapi.yml
- filename: portone-payment-schedules-api-openapi.yml
  format: yaml
  label: PortOne Payment Schedules API
  slug: portone-payment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-schedules-api-openapi.yml
- filename: portone-payment-sessions-api-openapi.yml
  format: yaml
  label: PortOne Payment Sessions API
  slug: portone-payment-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-sessions-api-openapi.yml
- filename: portone-payments-api-openapi.yml
  format: yaml
  label: PortOne Payments API
  slug: portone-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payments-api-openapi.yml
- filename: portone-payments-by-cursor-api-openapi.yml
  format: yaml
  label: PortOne Payments By Cursor API
  slug: portone-payments-by-cursor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payments-by-cursor-api-openapi.yml
- filename: portone-paymentwall-api-openapi.yml
  format: yaml
  label: PortOne Paymentwall API
  slug: portone-paymentwall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-paymentwall-api-openapi.yml
- filename: portone-platform-api-openapi.yml
  format: yaml
  label: PortOne Platform API
  slug: portone-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-platform-api-openapi.yml
- filename: portone-promotions-api-openapi.yml
  format: yaml
  label: PortOne Promotions API
  slug: portone-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-promotions-api-openapi.yml
- filename: portone-token-api-openapi.yml
  format: yaml
  label: PortOne Token API
  slug: portone-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-token-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Portone Authentication
name_suffix: Authentication
oauth_flows: []
overview: PortOne secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PortOne
provider_slug: portone
scheme_count: 3
schemes:
- description: V2 API Secret authentication. Custom "PortOne" Authorization scheme carrying the API Secret issued in the PortOne admin console.
  headerFormat: 'Authorization: PortOne <API_SECRET>'
  name: portOne
  scheme: portone
  sources:
  - openapi/portone-openapi.yml
  type: http
- description: V2 short-lived JWT access token, obtained by exchanging the API Secret via POST /login/api-secret. Preferred for browser-adjacent or delegated calls.
  headerFormat: 'Authorization: Bearer <accessToken>'
  name: bearerJwt
  scheme: bearer
  sources:
  - openapi/portone-openapi.yml
  type: http
- description: Legacy V1 (Iamport) token. POST /users/getToken with imp_key and imp_secret returns an access_token presented on subsequent api.iamport.kr requests.
  headerFormat: 'Authorization: <access_token>'
  name: v1Token
  scheme: bearer
  sources:
  - https://developers.portone.io/api/rest-v1
  type: http
slug: portone-authentication
source_filename: portone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/portone-openapi.yml\ndocs: https://developers.portone.io/api/rest-v2/auth\nsummary:\n  types:\n  - http\nnotes: >-\n  PortOne V2 (api.portone.io) authenticates with an API Secret passed in the\n  Authorization header using the custom scheme keyword \"PortOne\" (not \"Bearer\"):\n  `Authorization: PortOne <API_SECRET>`. The V2 API Secret is issued from the\n  PortOne admin console payment-integration tab. A short-lived access token can\n  also be exchanged (POST /login/api-secret) and presented as a JWT bearer token\n  (`Authorization: Bearer <accessToken>`). The legacy V1 API (api.iamport.kr) uses\n  a two-step token flow: POST /users/getToken with imp_key + imp_secret returns an\n  access_token that is then sent in the Authorization header.\nschemes:\n- name: portOne\n  type: http\n  scheme: portone\n  headerFormat: 'Authorization: PortOne <API_SECRET>'\n  description: >-\n    V2 API Secret authentication. Custom \"\
  PortOne\" Authorization scheme carrying\n    the API Secret issued in the PortOne admin console.\n  sources:\n  - openapi/portone-openapi.yml\n- name: bearerJwt\n  type: http\n  scheme: bearer\n  headerFormat: 'Authorization: Bearer <accessToken>'\n  description: >-\n    V2 short-lived JWT access token, obtained by exchanging the API Secret via\n    POST /login/api-secret. Preferred for browser-adjacent or delegated calls.\n  sources:\n  - openapi/portone-openapi.yml\n- name: v1Token\n  type: http\n  scheme: bearer\n  headerFormat: 'Authorization: <access_token>'\n  description: >-\n    Legacy V1 (Iamport) token. POST /users/getToken with imp_key and imp_secret\n    returns an access_token presented on subsequent api.iamport.kr requests.\n  sources:\n  - https://developers.portone.io/api/rest-v1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/authentication/portone-authentication.yml
summary_line: http · 3 schemes
tags:
- Payments
- Payment Orchestration
- Fintech
- Korea
- Billing
- Identity Verification
---
