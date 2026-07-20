---
api_key_in:
- header
api_specs:
- filename: didit-openapi-original.json
  format: json
  label: Didit Verification API
  slug: didit-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Didit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Didit secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Didit
provider_slug: didit
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
- description: Short-lived scoped token minted by your backend via POST /v3/transactions/sdk-token/. Used by the Didit SDKs on the device-facing /v1/transactions/ endpoints.
  in: header
  name: TransactionTokenAuth
  parameter: X-Transaction-Token
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
- description: Short-lived token returned in the `session_token` field of POST /v3/session/. Used by the hosted verification flow (and custom sandbox UIs) to call session-scoped endpoints on behalf of the verifying user, without your server-side API key.
  in: header
  name: SessionTokenAuth
  parameter: Session-Token
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
slug: didit-authentication
source_filename: didit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/didit-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/didit-openapi-original.json\n- name: TransactionTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Transaction-Token\n  description: Short-lived scoped token minted by your backend via POST /v3/transactions/sdk-token/.\n    Used by the Didit SDKs on the device-facing /v1/transactions/ endpoints.\n  sources:\n  - openapi/didit-openapi-original.json\n- name: SessionTokenAuth\n  type: apiKey\n  in: header\n  parameter: Session-Token\n  description: Short-lived token returned in the `session_token` field of POST /v3/session/.\n    Used by the hosted verification flow (and custom sandbox UIs) to call session-scoped endpoints\n    on behalf of the verifying user, without your server-side API key.\n  sources:\n  - openapi/didit-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/authentication/didit-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Compliance
- Biometrics
- Transaction Monitoring
- Crypto
---
