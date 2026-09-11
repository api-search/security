---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: First Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: First Data (Fiserv) secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: First Data (Fiserv)
provider_slug: first-data
scheme_count: 3
schemes:
- description: '"Key given to merchant after boarding associating their requests with the appropriate app in Apigee." Issued per merchant at onboarding; the gateway fronts on Apigee.'
  in: header
  name: Api-Key
  parameter: Api-Key
  required: true
  sources:
  - https://github.com/GBSEcom/Python
  type: apiKey
- algorithm: HMAC-SHA256
  description: '"Used to ensure the request has not been tampered with during transmission. The Message-Signature is the Base64 encoded HMAC hash (SHA256 algorithm with the API Secret as the key)." The signed string is the concatenation Api-Key + Client-Request-Id + Timestamp + the JSON request body.'
  encoding: base64
  name: Message-Signature
  parameter: Message-Signature
  required: true
  scheme: hmac
  sources:
  - https://github.com/GBSEcom/Python
  type: http
- description: Bearer access token obtained from POST /v2/authentication/access-tokens. Used for the browser/client-side flows (payment tokens, hosted payment pages) so that the API Secret never leaves the merchant server.
  name: Authorization
  parameter: Authorization
  required: false
  scheme: bearer
  sources:
  - https://github.com/GBSEcom/Python
  type: http
slug: first-data-authentication
source_filename: first-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: >-\n  First Data's own First Data Gateway (IPG) client libraries, published by the\n  GBSEcom organization: https://github.com/GBSEcom/java (README) and\n  https://github.com/GBSEcom/Python (simple/signature.py, simple/client_context.py,\n  openapi_client/api/*.py parameter documentation).\ndocs: https://developer.fiserv.com/product/IPGNA/\nnote: >-\n  The First Data Gateway publishes no OpenAPI document at any reachable URL (see\n  the contract-discovery record in this repo's apis.yml x-coverage block), so this\n  profile is read from the generated client libraries First Data itself published,\n  which carry the scheme names, header names, signing algorithm and parameter\n  descriptions verbatim from the source specification.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  request_signing: hmac-sha256\nschemes:\n  - name: Api-Key\n    type: apiKey\n    in: header\n    parameter: Api-Key\n\
  \    required: true\n    description: >-\n      \"Key given to merchant after boarding associating their requests with the\n      appropriate app in Apigee.\" Issued per merchant at onboarding; the gateway\n      fronts on Apigee.\n    sources: [https://github.com/GBSEcom/Python]\n  - name: Message-Signature\n    type: http\n    scheme: hmac\n    algorithm: HMAC-SHA256\n    encoding: base64\n    parameter: Message-Signature\n    required: true\n    description: >-\n      \"Used to ensure the request has not been tampered with during transmission.\n      The Message-Signature is the Base64 encoded HMAC hash (SHA256 algorithm with\n      the API Secret as the key).\" The signed string is the concatenation\n      Api-Key + Client-Request-Id + Timestamp + the JSON request body.\n    sources: [https://github.com/GBSEcom/Python]\n  - name: Authorization\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    required: false\n    description: >-\n      Bearer access token obtained\
  \ from POST /v2/authentication/access-tokens.\n      Used for the browser/client-side flows (payment tokens, hosted payment\n      pages) so that the API Secret never leaves the merchant server.\n    sources: [https://github.com/GBSEcom/Python]\nrequired_headers:\n  - name: Content-Type\n    description: application/json\n  - name: Client-Request-Id\n    description: >-\n      \"A client-generated ID for request tracking and signature creation, unique\n      per request. This is also used for idempotency control. We recommend 128-bit\n      UUID format.\"\n  - name: Api-Key\n    description: Merchant API key issued at boarding.\n  - name: Timestamp\n    description: >-\n      \"Epoch timestamp in milliseconds in the request from a client system. Used\n      for Message Signature generation and time limit (5 mins).\"\n  - name: Message-Signature\n    description: Base64-encoded HMAC-SHA256 of Api-Key + Client-Request-Id + Timestamp + body.\n  - name: Region\n    required: false\n    description:\
  \ >-\n      \"Indicates the region where the client wants the transaction to be\n      processed. This will override the default processing region identified for\n      the client. Available options are argentina, brazil, germany, india and\n      northamerica.\"\ncredentials:\n  - name: API Key\n    issued_at: merchant boarding\n  - name: API Secret\n    issued_at: merchant boarding\n    use: HMAC signing key only; never transmitted\ntoken_endpoint:\n  operation: POST /v2/authentication/access-tokens\n  description: Generate an access token for client-side/browser authentication.\n  request_fields: [domain, token, publicKeyRequired]\nenvironments:\n  - name: production\n    base_url: https://prod.api.firstdata.com/gateway/v2\n  - name: certification\n    base_url: https://cert.api.firstdata.com/gateway/v2\n    note: The SDKs default to the certification (sandbox) host.\ngaps:\n  - No OAuth 2.0 or OpenID Connect surface is documented for the First Data Gateway.\n  - No scope model exists,\
  \ so this repo carries no scopes/ artifact.\n  - >-\n    Credentials cannot be obtained self-service; an API Key and API Secret are\n    issued only through merchant boarding, which is a sales-gated process.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-data/refs/heads/main/authentication/first-data-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- Merchant Services
- Financial-Services
- Transaction Processing
- Fortune 500
---
