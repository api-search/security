---
api_key_in:
- header
api_specs:
- filename: qentaz-webhooks-asyncapi.yml
  format: yaml
  label: Trazo API
  slug: trazo-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qentaz/refs/heads/main/asyncapi/qentaz-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qentaz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qentaz secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qentaz
provider_slug: qentaz
scheme_count: 4
schemes:
- description: Static per-integration authentication key exchanged for a temporary access token. Presented as an HTTP Bearer credential to the token endpoint.
  format: Bearer {auth_key}
  header: Authorization
  name: authKeyBearer
  scheme: bearer
  type: http
  used_on: GET /token
- description: Short-lived access token returned by GET /token, sent on every protected request. Value is the access_token from the token response.
  in: header
  name: accessToken
  name_param: x-auth-token
  type: apiKey
  used_on: all protected endpoints (e.g. POST /transaction, GET /v1/merchant/transaction/)
- description: Optional business/account selector used with administered (managed / child) accounts to scope a request to a sub-account.
  in: header
  name: childId
  name_param: child-id
  required: false
  type: apiKey
- description: Trazo signs outbound webhook deliveries with a Bearer credential built from base64(client_id:client_secret_key) so your endpoint can verify authenticity.
  direction: inbound-to-your-endpoint
  format: Bearer base64(client_id:client_secret_key)
  in: header
  name: webhookSignature
  name_param: Authorization
  type: apiKey
slug: qentaz-authentication
source_filename: qentaz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qentaz.com/documentation/autenticacion/token\ndocs: https://docs.qentaz.com/documentation/autenticacion/token\nsummary:\n  types: [apiKey, http]\n  model: two-step-bearer\n  api_key_in: [header]\n  notes: >-\n    Two-step bearer authentication. A static, long-lived authentication key\n    (auth_key, issued per integration) is sent as an HTTP Bearer credential to\n    GET /token, which returns a short-lived access_token (expires_in seconds,\n    e.g. 3600). That access_token is then sent on every subsequent request in\n    the custom x-auth-token header. No OAuth2/OIDC discovery is published; the\n    auth_key is provisioned out of band. Administered (\"child\") accounts are\n    selected with an optional child-id header.\nschemes:\n- name: authKeyBearer\n  type: http\n  scheme: bearer\n  used_on: GET /token\n  header: Authorization\n  format: 'Bearer {auth_key}'\n  description: >-\n    Static per-integration authentication\
  \ key exchanged for a temporary access\n    token. Presented as an HTTP Bearer credential to the token endpoint.\n- name: accessToken\n  type: apiKey\n  in: header\n  name_param: x-auth-token\n  used_on: all protected endpoints (e.g. POST /transaction, GET /v1/merchant/transaction/)\n  description: >-\n    Short-lived access token returned by GET /token, sent on every protected\n    request. Value is the access_token from the token response.\n- name: childId\n  type: apiKey\n  in: header\n  name_param: child-id\n  required: false\n  description: >-\n    Optional business/account selector used with administered (managed / child)\n    accounts to scope a request to a sub-account.\n- name: webhookSignature\n  type: apiKey\n  in: header\n  name_param: Authorization\n  format: 'Bearer base64(client_id:client_secret_key)'\n  direction: inbound-to-your-endpoint\n  description: >-\n    Trazo signs outbound webhook deliveries with a Bearer credential built from\n    base64(client_id:client_secret_key)\
  \ so your endpoint can verify authenticity.\ntoken_endpoint:\n  method: GET\n  path: /token\n  response:\n    access_token: string\n    expires_in: integer (seconds)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qentaz/refs/heads/main/authentication/qentaz-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Payments
- Collections
- Disbursements
- Reconciliation
- Fintech
- Colombia
- Webhooks
- Fraud Prevention
- WhatsApp Payments
---
