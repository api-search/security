---
api_key_in:
- header
api_specs:
- filename: advance-intelligence-group-advance-ai-openapi.yml
  format: yaml
  label: ADVANCE.AI Open API
  slug: advanceai-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-intelligence-group/refs/heads/main/openapi/advance-intelligence-group-advance-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Advance Intelligence Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advance Intelligence Group secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Advance Intelligence Group
provider_slug: advance-intelligence-group
scheme_count: 1
schemes:
- description: Short-lived access token passed on every request. Obtained from POST /openapi/auth/ticket/v1/generate-token.
  in: header
  name: AccessToken
  parameter: X-ACCESS-TOKEN
  sources:
  - openapi/advance-intelligence-group-advance-ai-openapi.yml
  type: apiKey
slug: advance-intelligence-group-authentication
source_filename: advance-intelligence-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/advance-intelligence-group-advance-ai-openapi.yml\ndocs: https://doc.advance.ai/global_document_verification.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Two-step: obtain a short-lived access token by signing a request with your\n    accessKey + secretKey, then pass the token in the X-ACCESS-TOKEN header on\n    every API call.\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  description: >-\n    Short-lived access token passed on every request. Obtained from\n    POST /openapi/auth/ticket/v1/generate-token.\n  sources:\n  - openapi/advance-intelligence-group-advance-ai-openapi.yml\ntoken_flow:\n  endpoint: POST /openapi/auth/ticket/v1/generate-token\n  request:\n    accessKey: Account access key.\n    timestamp: 13-digit Unix epoch milliseconds.\n    signature: SHA256(accessKey + secretKey + timestamp).\n    periodSecond: Optional token\
  \ TTL in seconds (default 3600, range 60-86400).\n  response:\n    token: Value for the X-ACCESS-TOKEN header.\n    expiredTime: Unix expiry timestamp; re-request when expired.\nnotes:\n- No OAuth 2.0 or OpenID Connect; credentials are an accessKey/secretKey pair.\n- Signature-based token issuance prevents replay via the timestamp component.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advance-intelligence-group/refs/heads/main/authentication/advance-intelligence-group-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Identity Verification
- KYC
- AML
- Face Recognition
- OCR
- Artificial Intelligence
- Risk Management
- Singapore
---
