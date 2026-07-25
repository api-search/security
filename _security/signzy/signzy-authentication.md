---
api_key_in: []
api_specs:
- filename: signzy-authentication-api-openapi.yml
  format: yaml
  label: Signzy Authentication API
  slug: signzy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-authentication-api-openapi.yml
- filename: signzy-banking-api-openapi.yml
  format: yaml
  label: Signzy Banking API
  slug: signzy-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-banking-api-openapi.yml
- filename: signzy-identity-india-api-openapi.yml
  format: yaml
  label: Signzy Identity (India) API
  slug: signzy-identity-india-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-india-api-openapi.yml
- filename: signzy-identity-us-api-openapi.yml
  format: yaml
  label: Signzy Identity (US) API
  slug: signzy-identity-us-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-us-api-openapi.yml
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
