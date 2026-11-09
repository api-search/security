---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crosscheckapi-com-accept-api-openapi.yml
  format: yaml
  label: Crosscheck Accept API
  slug: crosscheckapi-com-accept-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-accept-api-openapi.yml
- filename: crosscheckapi-com-accept-lite-api-openapi.yml
  format: yaml
  label: Crosscheck Accept Lite API
  slug: crosscheckapi-com-accept-lite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-accept-lite-api-openapi.yml
- filename: crosscheckapi-com-acceptance-test-api-openapi.yml
  format: yaml
  label: Crosscheck acceptance test API
  slug: crosscheckapi-com-acceptance-test-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-acceptance-test-api-openapi.yml
- filename: crosscheckapi-com-checks-api-openapi.yml
  format: yaml
  label: Crosscheck Checks API
  slug: crosscheckapi-com-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-checks-api-openapi.yml
- filename: crosscheckapi-com-draft-review-api-openapi.yml
  format: yaml
  label: Crosscheck draft review API
  slug: crosscheckapi-com-draft-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-draft-review-api-openapi.yml
- filename: crosscheckapi-com-quote-api-openapi.yml
  format: yaml
  label: Crosscheck Quote API
  slug: crosscheckapi-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-quote-api-openapi.yml
- filename: crosscheckapi-com-receipts-api-openapi.yml
  format: yaml
  label: Crosscheck Receipts API
  slug: crosscheckapi-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-receipts-api-openapi.yml
- filename: crosscheckapi-com-sellercheck-api-openapi.yml
  format: yaml
  label: Crosscheck Sellercheck API
  slug: crosscheckapi-com-sellercheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-sellercheck-api-openapi.yml
- filename: crosscheckapi-com-sellerwatch-api-openapi.yml
  format: yaml
  label: Crosscheck Sellerwatch API
  slug: crosscheckapi-com-sellerwatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-sellerwatch-api-openapi.yml
- filename: crosscheckapi-com-skill-security-api-openapi.yml
  format: yaml
  label: Crosscheck skill security API
  slug: crosscheckapi-com-skill-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skill-security-api-openapi.yml
- filename: crosscheckapi-com-skillcheck-api-openapi.yml
  format: yaml
  label: Crosscheck Skillcheck API
  slug: crosscheckapi-com-skillcheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skillcheck-api-openapi.yml
- filename: crosscheckapi-com-skillcheck-lite-api-openapi.yml
  format: yaml
  label: Crosscheck Skillcheck Lite API
  slug: crosscheckapi-com-skillcheck-lite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skillcheck-lite-api-openapi.yml
- filename: crosscheckapi-com-w-api-openapi.yml
  format: yaml
  label: Crosscheck W API
  slug: crosscheckapi-com-w-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-w-api-openapi.yml
- filename: crosscheckapi-com-x402-seller-api-openapi.yml
  format: yaml
  label: Crosscheck x402 seller API
  slug: crosscheckapi-com-x402-seller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-x402-seller-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crosscheckapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crosscheck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crosscheck
provider_slug: crosscheckapi-com
scheme_count: 1
schemes:
- description: 'x402 v2: send PAYMENT-SIGNATURE after the 402 challenge'
  name: x402
  scheme: bearer
  sources:
  - openapi/crosscheckapi-com-openapi.json
  type: http
slug: crosscheckapi-com-authentication
source_filename: crosscheckapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/crosscheckapi-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: x402\n  type: http\n  scheme: bearer\n  description: 'x402 v2: send PAYMENT-SIGNATURE after the 402 challenge'\n  sources:\n  - openapi/crosscheckapi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/crosscheckapi-com/authentication/crosscheckapi-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Verification
- Payments
- x402
- Blockchain
---
