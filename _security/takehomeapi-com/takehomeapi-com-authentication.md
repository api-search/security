---
anonymous_access: false
api_key_in: []
api_specs:
- filename: takehomeapi-com-compare-api-openapi.yml
  format: yaml
  label: takehomeapi-com Compare API
  slug: takehomeapi-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/takehomeapi-com/openapi/takehomeapi-com-compare-api-openapi.yml
- filename: takehomeapi-com-rates-api-openapi.yml
  format: yaml
  label: takehomeapi-com Rates API
  slug: takehomeapi-com-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/takehomeapi-com/openapi/takehomeapi-com-rates-api-openapi.yml
- filename: takehomeapi-com-take-home-api-openapi.yml
  format: yaml
  label: takehomeapi-com Take Home API
  slug: takehomeapi-com-take-home-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/takehomeapi-com/openapi/takehomeapi-com-take-home-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Takehomeapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: takehomeapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: takehomeapi-com
provider_slug: takehomeapi-com
scheme_count: 2
schemes:
- description: 'Free key: 100 calls/month. Also accepted as Authorization: Bearer <key>.'
  in: header
  name: X-API-Key
  type: apiKey
- description: Pay per call with x402 (USDC on Base), no account needed.
  in: header
  name: PAYMENT-SIGNATURE
  type: apiKey
slug: takehomeapi-com-authentication
source_filename: takehomeapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://takehomeapi.com/llms.txt\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"Free key: 100 calls/month. Also accepted as Authorization: Bearer <key>.\"\n  - type: apiKey\n    name: PAYMENT-SIGNATURE\n    in: header\n    description: \"Pay per call with x402 (USDC on Base), no account needed.\"\n"
source_yaml_url: https://artifacts.apis.io/takehomeapi-com/authentication/takehomeapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- UK
- Finance
- Tax
- Payroll
---
