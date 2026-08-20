---
api_key_in:
- header
api_specs:
- filename: lendapi-amortization-api-openapi.yml
  format: yaml
  label: LendAPI Amortization API
  slug: lendapi-amortization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-amortization-api-openapi.yml
- filename: lendapi-application-api-openapi.yml
  format: yaml
  label: LendAPI Application API
  slug: lendapi-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-application-api-openapi.yml
- filename: lendapi-credit-risk-api-openapi.yml
  format: yaml
  label: LendAPI Credit Risk API
  slug: lendapi-credit-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-credit-risk-api-openapi.yml
- filename: lendapi-decision-api-openapi.yml
  format: yaml
  label: LendAPI Decision API
  slug: lendapi-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-decision-api-openapi.yml
- filename: lendapi-decisions-api-openapi.yml
  format: yaml
  label: LendAPI Decisions API
  slug: lendapi-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-decisions-api-openapi.yml
- filename: lendapi-get-app-credit-report-api-openapi.yml
  format: yaml
  label: LendAPI Get App Credit Report API
  slug: lendapi-get-app-credit-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-get-app-credit-report-api-openapi.yml
- filename: lendapi-outcomes-api-openapi.yml
  format: yaml
  label: LendAPI Outcomes API
  slug: lendapi-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-outcomes-api-openapi.yml
- filename: lendapi-page-submit-api-openapi.yml
  format: yaml
  label: LendAPI Page Submit API
  slug: lendapi-page-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-page-submit-api-openapi.yml
- filename: lendapi-pricing-engine-api-openapi.yml
  format: yaml
  label: LendAPI Pricing Engine API
  slug: lendapi-pricing-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-pricing-engine-api-openapi.yml
- filename: lendapi-pricing-engines-api-openapi.yml
  format: yaml
  label: LendAPI Pricing Engines API
  slug: lendapi-pricing-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-pricing-engines-api-openapi.yml
- filename: lendapi-sub-tenant-api-openapi.yml
  format: yaml
  label: LendAPI Sub Tenant API
  slug: lendapi-sub-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-sub-tenant-api-openapi.yml
- filename: lendapi-sub-tenants-api-openapi.yml
  format: yaml
  label: LendAPI Sub Tenants API
  slug: lendapi-sub-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-sub-tenants-api-openapi.yml
- filename: lendapi-variable-api-openapi.yml
  format: yaml
  label: LendAPI Variable API
  slug: lendapi-variable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-variable-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lendapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: LendAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LendAPI
provider_slug: lendapi
scheme_count: 1
schemes:
- applied: global
  default_example: Bearer [example key]
  in: header
  name: sec0
  parameter: AUTHORIZATION
  sources:
  - openapi/lendapi-openapi.json
  type: apiKey
  value_format: Bearer <api_key>
slug: lendapi-authentication
source_filename: lendapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lendapi-openapi.json\ndocs: https://developer.lendapi.com/reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  value_format: 'Bearer <api_key>'\n  default_example: Bearer [example key]\n  applied: global\n  sources:\n  - openapi/lendapi-openapi.json\nenvironment_selection:\n  mechanism: api-key\n  modes:\n  - test\n  - live\n  detail: >-\n    \"The mode in which your request operates, either live or test, is determined by the\n    API key used for authentication.\" One header, one host -- the key alone decides\n    whether the call touches live data.\n  source: https://developer.lendapi.com/reference/introduction\nnotes: >-\n  LendAPI uses a single API-key scheme applied globally to all 20 published\n  operations. The header is spelled AUTHORIZATION and the value is bearer-formatted,\n\
  \  but the scheme is declared as apiKey rather than http/bearer in the definition.\n  There is no OAuth 2.0, no OpenID Connect, no mTLS, and therefore no scope or\n  consent model -- see conventions/lendapi-conventions.yml. Key rotation, expiry and\n  provisioning are not documented in the public developer portal; keys are issued\n  through the LendAPI application at https://app.lendapi.com/login/.\ngaps:\n- No 401 or 403 response is documented on any operation.\n- No key rotation, expiry, or revocation policy is published.\n- No scope, permission, or least-privilege model exists for keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/authentication/lendapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Lending
- Loan Origination
- Financial-Services
- Fintech
- Embedded Finance
- Underwriting
- Decision Engine
- Credit
- Banking
- Account Opening
- KYC
- KYB
- Buy Now Pay Later
- Point-of-Sale
---
