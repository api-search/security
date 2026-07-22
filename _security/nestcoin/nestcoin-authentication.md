---
api_key_in:
- header
- query
api_specs:
- filename: nestcoin-external-gateway-openapi-original.json
  format: json
  label: Onboard External API Gateway
  slug: onboard-external-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nestcoin/refs/heads/main/openapi/nestcoin-external-gateway-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nestcoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nestcoin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nestcoin
provider_slug: nestcoin
scheme_count: 2
schemes:
- in: header
  name: authSignature
  parameter: x-signature
  sources:
  - openapi/nestcoin-external-gateway-openapi-original.json
  type: apiKey
- description: Auth Token header for inter-service communication
  in: header
  name: authToken
  parameter: x-auth-token
  sources:
  - openapi/nestcoin-external-gateway-openapi-original.json
  type: apiKey
slug: nestcoin-authentication
source_filename: nestcoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nestcoin-external-gateway-openapi-original.json\ndocs: https://docs.onboard.xyz/api-reference/onboard-connect/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nmodels:\n  - name: API Key\n    headers: [x-api-key]\n    query: [x-api-key]\n    detail: Identifies the third-party application. Retrieved from the Business Dashboard after onboarding.\n  - name: Session token (x-auth-token)\n    headers: [x-auth-token, 'Authorization: Bearer <token>']\n    detail: Issued to an end user after OTP login; used for authenticated user-session endpoints.\n  - name: HMAC signature (x-signature)\n    headers: [x-api-key, x-signature, x-timestamp]\n    detail: >-\n      Sensitive operations (e.g. user creation) require HMAC-SHA256 signing. The signature is\n      computed over the x-timestamp and request body using the API secret as the key. Timestamps\n      must be within 30 seconds of server time\
  \ or the request is rejected with 403.\nschemes:\n- name: authSignature\n  type: apiKey\n  in: header\n  parameter: x-signature\n  sources:\n  - openapi/nestcoin-external-gateway-openapi-original.json\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: x-auth-token\n  description: Auth Token header for inter-service communication\n  sources:\n  - openapi/nestcoin-external-gateway-openapi-original.json\naccess_token_flow:\n  request_operation: requestAccessToken\n  refresh_operation: refreshAccessToken\n  path: /auth/oauth/access-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nestcoin/refs/heads/main/authentication/nestcoin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fintech
- Crypto
- Exchange
- On-Off Ramp
- Payments
- Web3
- Africa
---
