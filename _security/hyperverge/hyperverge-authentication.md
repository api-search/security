---
api_key_in: []
api_specs:
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge KYC OCR API
  slug: hyperverge-kyc-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Database Verification API
  slug: hyperverge-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Input Validation API
  slug: hyperverge-input-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Matching API
  slug: hyperverge-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Face Match API
  slug: hyperverge-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hyperverge Authentication
name_suffix: Authentication
oauth_flows: []
overview: HyperVerge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HyperVerge
provider_slug: hyperverge
scheme_count: 1
schemes:
- description: 'HyperVerge issues an `appId` and `appKey` pair after enterprise onboarding. Both are sent as request headers on every call: `appId` and `appKey` on the KYC OCR (ind-docs.hyperverge.co) and Verification (ind-verify.hyperverge.co) hosts, and lowercase `appid` and `appkey` on the Face Match (ind-faceid.hyperverge.co) host. Credentials are not self-serve - they are provided by the HyperVerge team. Invalid or missing credentials return HTTP 401. HyperVerge warns against exposing appId/appKey in browser applications; call the APIs server-side.'
  headers:
  - appId
  - appKey
  - appid
  - appkey
  in: header
  name: appIdKey
  optionalHeaders:
  - description: Client-supplied identifier echoed back in responses for request grouping.
    name: referenceId
  - description: Enables an X-Response-Signature checksum header for response integrity validation.
    name: uuid
  - description: Optional transaction identifier on the Matching API.
    name: transactionid
  scheme: custom-header-pair
  sources:
  - openapi/hyperverge-openapi.yml
  - https://github.com/hyperverge/kyc-india-rest-api
  - https://github.com/hyperverge/face-match-india-rest-api
  type: apiKey
slug: hyperverge-authentication
source_filename: hyperverge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/hyperverge-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: appIdKey\n  type: apiKey\n  in: header\n  scheme: custom-header-pair\n  description: >-\n    HyperVerge issues an `appId` and `appKey` pair after enterprise onboarding.\n    Both are sent as request headers on every call: `appId` and `appKey` on the\n    KYC OCR (ind-docs.hyperverge.co) and Verification (ind-verify.hyperverge.co)\n    hosts, and lowercase `appid` and `appkey` on the Face Match\n    (ind-faceid.hyperverge.co) host. Credentials are not self-serve - they are\n    provided by the HyperVerge team. Invalid or missing credentials return HTTP\n    401. HyperVerge warns against exposing appId/appKey in browser applications;\n    call the APIs server-side.\n  headers:\n  - appId\n  - appKey\n  - appid\n  - appkey\n  optionalHeaders:\n  - name: referenceId\n    description: Client-supplied identifier echoed back in responses for request grouping.\n\
  \  - name: uuid\n    description: Enables an X-Response-Signature checksum header for response integrity validation.\n  - name: transactionid\n    description: Optional transaction identifier on the Matching API.\n  sources:\n  - openapi/hyperverge-openapi.yml\n  - https://github.com/hyperverge/kyc-india-rest-api\n  - https://github.com/hyperverge/face-match-india-rest-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/authentication/hyperverge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Verification
- KYC
- Face Authentication
- Liveness
- Document Verification
- India
- AML
- Onboarding
- Fraud Prevention
- AI
---
