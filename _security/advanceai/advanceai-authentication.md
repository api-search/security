---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: advanceai-openapi.yml
  format: yaml
  label: ADVANCE.AI Open API
  slug: advanceai-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Advanceai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADVANCE.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ADVANCE.AI
provider_slug: advanceai
scheme_count: 1
schemes:
- description: Short-lived access token obtained from POST /openapi/auth/ticket/v1/generate-token and passed on every other operation. One token is valid across all ADVANCE.AI Open APIs and is reusable until it expires. Requesting a new token does NOT invalidate an outstanding one.
  in: header
  name: AccessToken
  parameter: X-ACCESS-TOKEN
  sources:
  - openapi/advanceai-openapi.yml
  - https://doc.advance.ai/liveness_detection.html
  type: apiKey
slug: advanceai-authentication
source_filename: advanceai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://doc.advance.ai/global_document_verification.html\ndocs: https://doc.advance.ai/global_document_verification.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth: false\n  openid_connect: false\n  mtls: false\n  note: >-\n    ADVANCE.AI uses a signed key-exchange followed by a bearer-style header token. There is no OAuth\n    2.0, no OpenID Connect and no documented mTLS, so there is no scope surface — see the absence of\n    scopes/ in this repo, which is correct rather than missing.\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  description: >-\n    Short-lived access token obtained from POST /openapi/auth/ticket/v1/generate-token and passed on\n    every other operation. One token is valid across all ADVANCE.AI Open APIs and is reusable until\n    it expires. Requesting a new token does NOT invalidate an outstanding one.\n  sources:\n  - openapi/advanceai-openapi.yml\n\
  \  - https://doc.advance.ai/liveness_detection.html\ncredentials:\n  issued_via: >-\n    accessKey and secretKey are issued per account and read from the ADVANCE.AI Websaas platform\n    under Account > Account Management. There is no self-service key issuance — access is sales-led\n    via https://advance.ai/book-free-demo/.\n  key_pair:\n  - name: accessKey\n    role: public identifier, sent in the token request body\n  - name: secretKey\n    role: shared secret, never transmitted; used only to compute the signature\ntoken_exchange:\n  operation_id: generateAccessToken\n  method: POST\n  url: https://api.advance.ai/openapi/auth/ticket/v1/generate-token\n  unauthenticated: true\n  request_fields:\n  - name: accessKey\n    required: true\n  - name: signature\n    required: true\n    description: SHA256 hex digest of the concatenation accessKey + secretKey + timestamp.\n  - name: timestamp\n    required: true\n    description: >-\n      13-digit epoch milliseconds. Must be the same value\
  \ used inside the signature. ADVANCE.AI\n      suggests staying within 300 seconds of current time; a stale value returns\n      PARAMETER_ERROR \"Timestamp error\".\n  - name: periodSecond\n    required: false\n    description: Requested token lifetime in seconds. Default 3600, minimum 60, maximum 86400.\n  signature_algorithm: SHA256\n  signature_recipe: SHA256(accessKey || secretKey || timestamp)\n  response_fields:\n  - token\n  - expiredTime\n  token_lifetime_seconds:\n    default: 3600\n    min: 60\n    max: 86400\nfailure_modes:\n- code: PARAMETER_ERROR\n  meaning: Missing field, \"Timestamp error\", or \"Signature error\".\n  billed: false\n- code: ACCOUNT_DISABLED\n  meaning: Account Disabled — contact the ADVANCE.AI sales manager.\n  billed: false\n- code: IAM_FAILED\n  meaning: >-\n    Returned by the business operations rather than the token endpoint. Covers \"Token not found or\n    expired\", \"Access Key not found or expired\", \"Account not authorized for this country\"\
  ,\n    \"Account not authorized for this domain\", \"Account is expired\" and \"Account is disabled\".\n  billed: false\nnotes:\n- >-\n  The HTTP status is 200 even for authentication failure. Clients must branch on the envelope `code`\n  field, never on the HTTP status.\n- >-\n  ADVANCE.AI explicitly advises re-obtaining a token when the previous one expires, and states the\n  token is shared across every Open API, so one token cache serves the whole integration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/authentication/advanceai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Face Recognition
- Liveness Detection
- OCR
- Document Verification
- Risk Management
- Artificial Intelligence
- Fintech
- Singapore
---
