---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Abiglobalhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abi Global Health declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Abi Global Health
provider_slug: abiglobalhealth
scheme_count: 3
schemes:
- description: The long-lived partner credential. It is NOT sent on ordinary API calls — it is exchanged in the request body of the token endpoint for a short-lived access token.
  handling_guidance: '"Do not share your secret API key or any account information in publicly accessible areas such as GitHub, client-side code, and so forth."'
  id: partner-api-key
  in: body
  name: apiKey
  type: apiKey
  used_at: POST https://client-api.abi.ai/partner/authorization/token
- description: 'The access_token returned by the token endpoint, sent as `Authorization: Bearer <access_token>` on all protected endpoints. token_type is always "Bearer".'
  expiry_behavior: '"If the access_token is expired, the API will return a 401 Unauthorized response."'
  id: bearer-access-token
  in: header
  name: Authorization
  scheme: bearer
  ttl_seconds: 3600
  type: http
- description: The refresh_token returned alongside the access token, exchanged at the refresh endpoint for a new access token.
  expiry_behavior: '"If the refresh token expires, a new API key authentication is required."'
  id: refresh-token
  scheme: bearer
  ttl_hours: 24
  type: http
  used_at: POST https://client-api.abi.ai/partner/authorization/token/refresh
slug: abiglobalhealth-authentication
source_filename: abiglobalhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.abi.ai/ (Abi API Reference — \"Getting Started\" and \"Authentication\" sections)\nnote: >-\n  Abi publishes no OpenAPI/Swagger document, so this profile is read from the provider's own public\n  API reference at docs.abi.ai rather than derived from securitySchemes. Every statement below is\n  taken verbatim from that reference.\napi: Abi API\ndocs: https://docs.abi.ai/\nonboarding:\n  model: partner-gated\n  steps:\n  - Apply for a partner account through the docs \"Apply for Partner Account\" form.\n  - Abi evaluates the request and contacts the applicant with an API key.\n  - A test partner account is issued first; full integration requires contacting the sales team.\n  quote: >-\n    \"After you apply for an account, we will evaluate your request and contact you with your API\n    key. Once you have tested the service, if you decide to integrate fully with Abi, please\n    contact our sales team.\"\nschemes:\n\
  - id: partner-api-key\n  type: apiKey\n  in: body\n  name: apiKey\n  description: >-\n    The long-lived partner credential. It is NOT sent on ordinary API calls — it is exchanged in\n    the request body of the token endpoint for a short-lived access token.\n  used_at: POST https://client-api.abi.ai/partner/authorization/token\n  handling_guidance: >-\n    \"Do not share your secret API key or any account information in publicly accessible areas such\n    as GitHub, client-side code, and so forth.\"\n- id: bearer-access-token\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  description: >-\n    The access_token returned by the token endpoint, sent as `Authorization: Bearer <access_token>`\n    on all protected endpoints. token_type is always \"Bearer\".\n  ttl_seconds: 3600\n  expiry_behavior: >-\n    \"If the access_token is expired, the API will return a 401 Unauthorized response.\"\n- id: refresh-token\n  type: http\n  scheme: bearer\n  description: >-\n    The\
  \ refresh_token returned alongside the access token, exchanged at the refresh endpoint for a\n    new access token.\n  used_at: POST https://client-api.abi.ai/partner/authorization/token/refresh\n  ttl_hours: 24\n  expiry_behavior: >-\n    \"If the refresh token expires, a new API key authentication is required.\"\ntoken_endpoints:\n- operation: create-token\n  method: POST\n  url: https://client-api.abi.ai/partner/authorization/token\n  request: API key in the request body\n  response_fields:\n  - name: access_token\n    description: Your access token, used in the authorization header.\n  - name: token_type\n    description: The type of token returned. Always \"Bearer\".\n  - name: refresh_token\n    description: Your refresh token, used to obtain a new access token.\n- operation: refresh-token\n  method: POST\n  url: https://client-api.abi.ai/partner/authorization/token/refresh\nsub_partners:\n  supported: true\n  description: >-\n    \"Subpartners can authenticate using the same process\
  \ as partners, but must include their\n    subPartnerName in the request body.\" The same applies to the refresh call.\n  parameter:\n    name: subPartnerName\n    type: string\n    required: false\n    example: SubPartnerName_TEST\n    description: >-\n      The name of the partner (company) in Abi's system to which the user is assigned. Also used to\n      distinguish test partners from production partners.\nstandards:\n  oauth2: false\n  oidc: false\n  note: >-\n    The flow is bearer-token-shaped and access/refresh-token-shaped but is NOT an OAuth 2.0\n    implementation — Abi publishes no /token grant_type vocabulary, no scopes, no authorization\n    endpoint, and no /.well-known/oauth-authorization-server (probed 2026-09-06, 404 on every host).\n    Recorded as a proprietary API-key-for-bearer-token exchange, not oauth2.\nscopes:\n  published: false\n  note: >-\n    No scope or permission reference is published. Access differences are configured per partner\n    account server-side\
  \ — the 403 status description reads \"your partner configuration does not\n    allow the requested action\". scopes/ is therefore intentionally absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abiglobalhealth/refs/heads/main/authentication/abiglobalhealth-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Telehealth
- Virtual Care
- Digital Health
- Health Insurance
- Healthcare Navigation
- Artificial Intelligence
- Prescriptions
- Webhooks
- Ireland
---
