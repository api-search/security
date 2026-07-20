---
api_key_in: []
api_specs:
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy Identity Verification API
  slug: signzy-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy Aadhaar Verification API
  slug: signzy-aadhaar-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy PAN Verification API
  slug: signzy-pan-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy US Document Intelligence API
  slug: signzy-us-document-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy Business Verification (KYB) API
  slug: signzy-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy AML & Sanctions Screening API
  slug: signzy-aml-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy Bank Verification & Account Aggregator API
  slug: signzy-bank-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy Video KYC API
  slug: signzy-video-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
- filename: signzy-openapi.yml
  format: yaml
  label: Signzy eSign & Digital Contracting API
  slug: signzy-esign-contracting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signzy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signzy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Signzy
provider_slug: signzy
scheme_count: 1
schemes:
- format: raw-token
  header: Authorization
  in: header
  name: accessToken
  sources:
  - openapi/signzy-openapi.yml
  - https://docs.signzy.com/investor-onboarding-io/authentication
  - https://docs.signzy.com/generic-onboarding/login-api
  tokenEndpoint: /api/customers/login
  type: apiKey
slug: signzy-authentication
source_filename: signzy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/signzy-openapi.yml\nsummary:\n  types:\n  - apiKey\nnotes: >-\n  Signzy uses a LoopBack-style token flow. Clients POST a username and API key\n  (as password) to /api/customers/login and receive an access token in the `id`\n  field of the response (with `ttl` and `created`). That token is then sent as\n  the RAW value of the `Authorization` header on subsequent calls - NOT a\n  Bearer token and NOT an HTTP Basic credential. A `?access_token=` query\n  parameter is also accepted but discouraged. Confirmed live: api.signzy.app\n  returns HTTP 401 at root (auth required) on probe 2026-07-17.\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  header: Authorization\n  format: raw-token\n  tokenEndpoint: /api/customers/login\n  sources:\n  - openapi/signzy-openapi.yml\n  - https://docs.signzy.com/investor-onboarding-io/authentication\n  - https://docs.signzy.com/generic-onboarding/login-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/authentication/signzy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Verification
- KYC
- KYB
- AML
- Onboarding
- Compliance
- RegTech
---
