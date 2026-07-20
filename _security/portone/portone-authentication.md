---
api_key_in: []
api_specs:
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payments API (V2)
  slug: portone-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Billing Keys API (V2)
  slug: portone-billing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Schedule API (V2)
  slug: portone-payment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Identity Verification API (V2)
  slug: portone-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Cash Receipts API (V2)
  slug: portone-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne B2B Tax Invoice API (V2)
  slug: portone-b2b-tax-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Platform Partner Settlement API (V2)
  slug: portone-platform-partner-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Sessions & Checkout API (V2)
  slug: portone-payment-sessions-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Reconciliation API (V2)
  slug: portone-payment-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
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
