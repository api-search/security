---
api_key_in:
- body
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Flash Express Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flash Express secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flash Express
provider_slug: flash-express
scheme_count: 1
schemes:
- algorithm: SHA256
  content_type: application/x-www-form-urlencoded
  encoding: uppercase hex
  failure:
    code: 1002
    message: invalid signature
    source: https://open-docs.flashexpress.com/#response-code
  in: body
  name: FlashSignature
  parameters:
  - description: Merchant account number issued by Flash Express.
    name: mchId
    required: true
    type: string(32)
  - description: Random nonce string, included so the signature is unpredictable. The documentation recommends generating a random number and converting it to a string; the published examples also use millisecond epoch timestamps.
    name: nonceStr
    required: true
    type: string(32)
  - description: Uppercase SHA256 signature over the canonicalized request.
    name: sign
    required: true
    type: string(64)
  request_method: POST
  response_signing:
    note: Webhook callbacks delivered to the merchant are themselves signed. For webhook requests only mchId and nonceStr participate in the signature, so a merchant verifying an inbound webhook signs a different parameter set than it does when calling the API.
    supported: true
  secret:
    issuance: 'The merchant secret key is issued and reset only by Flash Express support staff. The documentation states "About The security key: Please contact the official support staff to obtain or reset." There is no self-service key provisioning.'
    name: key
    rotation_documented: false
  signing_algorithm:
    excluded_from_signature:
    - the sign parameter itself
    - any parameter whose value is entirely whitespace. The documentation enumerates the whitespace characters as HORIZONTAL TABULATION (U+0009), LINE FEED (U+000A), VERTICAL TABULATION (U+000B), FORM FEED (U+000C), ENTER (U+000D), FILE SEPARATOR (U+001C), GROUP SEPARATOR (U+001D), RECORD SEPARATOR (U+001E) and UNIT SEPARATOR (U+001F).
    forward_compatibility: The documentation states the API may add fields and that verifiers must support newly added extended fields when checking a signature.
    steps:
    - Collect every sent parameter into set M.
    - Drop any parameter whose value is empty or consists only of whitespace; blank values may still be transmitted but must not be signed.
    - Sort the remaining parameter names by ASCII code, ascending (dictionary order). Parameter names are case sensitive.
    - Join as key1=value1&key2=value2 into stringA.
    - Append the merchant secret as &key=<secret> to produce stringSignTemp.
    - sign = SHA256(stringSignTemp) uppercased.
    - Compute the signature BEFORE urlencoding; the server verifies after urldecoding.
  transport: https
  type: signature
slug: flash-express-authentication
source_filename: flash-express-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://open-docs.flashexpress.com/#the-security-reference\ndocs: https://open-docs.flashexpress.com/#signature-algorithm\nnote: >-\n  Flash Express publishes no OpenAPI, so this profile was read directly from the published\n  \"The Security Reference\" section of the FlashExpress Open API documentation rather than\n  derived from securitySchemes. The scheme is a shared-secret request-signing model, not a\n  bearer token and not OAuth: there is no token endpoint, no authorization server, no\n  scopes, and no refresh flow. Every request carries the merchant identity inline and is\n  signed per-call.\nsummary:\n  types: [signature]\n  api_key_in: [body]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer_token: false\nschemes:\n- name: FlashSignature\n  type: signature\n  in: body\n  transport: https\n  request_method: POST\n  content_type: application/x-www-form-urlencoded\n  algorithm:\
  \ SHA256\n  encoding: uppercase hex\n  parameters:\n  - name: mchId\n    type: string(32)\n    required: true\n    description: Merchant account number issued by Flash Express.\n  - name: nonceStr\n    type: string(32)\n    required: true\n    description: >-\n      Random nonce string, included so the signature is unpredictable. The documentation\n      recommends generating a random number and converting it to a string; the published\n      examples also use millisecond epoch timestamps.\n  - name: sign\n    type: string(64)\n    required: true\n    description: Uppercase SHA256 signature over the canonicalized request.\n  secret:\n    name: key\n    issuance: >-\n      The merchant secret key is issued and reset only by Flash Express support staff.\n      The documentation states \"About The security key: Please contact the official\n      support staff to obtain or reset.\" There is no self-service key provisioning.\n    rotation_documented: false\n  signing_algorithm:\n    steps:\n\
  \    - Collect every sent parameter into set M.\n    - Drop any parameter whose value is empty or consists only of whitespace; blank values may still be transmitted but must not be signed.\n    - Sort the remaining parameter names by ASCII code, ascending (dictionary order). Parameter names are case sensitive.\n    - Join as key1=value1&key2=value2 into stringA.\n    - Append the merchant secret as &key=<secret> to produce stringSignTemp.\n    - sign = SHA256(stringSignTemp) uppercased.\n    - Compute the signature BEFORE urlencoding; the server verifies after urldecoding.\n    excluded_from_signature:\n    - the sign parameter itself\n    - >-\n      any parameter whose value is entirely whitespace. The documentation enumerates the\n      whitespace characters as HORIZONTAL TABULATION (U+0009), LINE FEED (U+000A),\n      VERTICAL TABULATION (U+000B), FORM FEED (U+000C), ENTER (U+000D), FILE SEPARATOR\n      (U+001C), GROUP SEPARATOR (U+001D), RECORD SEPARATOR (U+001E) and UNIT SEPARATOR\n\
  \      (U+001F).\n    forward_compatibility: >-\n      The documentation states the API may add fields and that verifiers must support\n      newly added extended fields when checking a signature.\n  response_signing:\n    supported: true\n    note: >-\n      Webhook callbacks delivered to the merchant are themselves signed. For webhook\n      requests only mchId and nonceStr participate in the signature, so a merchant\n      verifying an inbound webhook signs a different parameter set than it does when\n      calling the API.\n  failure:\n    code: 1002\n    message: invalid signature\n    source: https://open-docs.flashexpress.com/#response-code\nsub_accounts:\n  supported: true\n  operation: POST /open/v1/new_sub_account\n  note: Merchants can create sub-accounts, each of which receives its own merchant credentials.\nenvironments:\n- name: production\n  base_url: https://open-api.flashexpress.com\n- name: training\n  base_url: https://open-api-tra.flashexpress.com\n  note: Separate\
  \ credentials are issued per environment by Flash Express support.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flash-express/refs/heads/main/authentication/flash-express-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Delivery
- Parcel Tracking
- E-Commerce
- Last Mile
- Courier
- Cash on Delivery
- Thailand
- Southeast Asia
- Webhooks
---
