---
api_key_in: []
api_specs:
- filename: serbia-company-data-company-api-openapi.yml
  format: yaml
  label: Serbia Company Data Company API
  slug: serbia-company-data-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/openapi/serbia-company-data-company-api-openapi.yml
- filename: serbia-company-data-search-api-openapi.yml
  format: yaml
  label: Serbia Company Data Search API
  slug: serbia-company-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/openapi/serbia-company-data-search-api-openapi.yml
auth_types:
- none
- x402-payment
description: ''
kind: authentication
layout: security
method: searched
name: Serbia Company Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Serbia Company Data secures its APIs with none and x402-payment across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Serbia Company Data
provider_slug: serbia-company-data
scheme_count: 1
schemes:
- accepts:
  - asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    asset_name: USD Coin
    asset_version: '2'
    max_timeout_seconds: 300
    network: eip155:8453
    network_name: Base
    pay_to: '0xcEE09f451355261E5f6a0271757638A55AF8Ae7b'
    scheme: exact
  challenge_header: PAYMENT-REQUIRED
  challenge_status: 402
  encoding: base64-encoded JSON
  extensions:
  - name: bazaar
    note: Each 402 challenge carries a bazaar discovery block with the route's input/output example and a JSON Schema 2020-12 document — harvested to json-schema/.
  name: x402
  protocol: x402
  request_header: PAYMENT-SIGNATURE
  settlement_header: PAYMENT-RESPONSE
  sources:
  - openapi/_original/serbia-company-data-openapi.json
  spec: https://github.com/x402-foundation/x402/blob/main/specs/transports-v2/http.md
  transport: http
  type: payment
  version: 2
slug: serbia-company-data-authentication
source_filename: serbia-company-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://serbia-company-x402.vercel.app/ + live PAYMENT-REQUIRED header capture\ndocs: https://docs.x402.org/getting-started/quickstart-for-buyers\nsummary:\n  types: [none, x402-payment]\n  api_key_in: []\n  oauth2_flows: []\n  accounts_required: false\n  api_keys_required: false\nnotes: >-\n  This API has no identity-based authentication. There is no account, no signup, no API key and no\n  OAuth. Authorization is per-request and economic: an unpaid call to a priced route returns\n  HTTP 402 with an x402 v2 payment challenge, and the caller re-sends the request carrying a signed\n  payment payload. The OpenAPI declares no securitySchemes, which is a faithful reflection of that\n  model rather than an omission — but it also means the payment contract is invisible to any tool\n  that reads only the spec's security section (see gaps).\nschemes:\n  - name: x402\n    type: payment\n    protocol: x402\n    version: 2\n    transport:\
  \ http\n    request_header: PAYMENT-SIGNATURE\n    challenge_header: PAYMENT-REQUIRED\n    settlement_header: PAYMENT-RESPONSE\n    challenge_status: 402\n    encoding: base64-encoded JSON\n    sources: [openapi/_original/serbia-company-data-openapi.json]\n    spec: https://github.com/x402-foundation/x402/blob/main/specs/transports-v2/http.md\n    accepts:\n      - scheme: exact\n        network: eip155:8453\n        network_name: Base\n        asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n        asset_name: USD Coin\n        asset_version: '2'\n        pay_to: '0xcEE09f451355261E5f6a0271757638A55AF8Ae7b'\n        max_timeout_seconds: 300\n    extensions:\n      - name: bazaar\n        note: >-\n          Each 402 challenge carries a bazaar discovery block with the route's input/output example\n          and a JSON Schema 2020-12 document — harvested to json-schema/.\nunauthenticated_operations:\n  - path: /api/sample\n    method: get\n    note: Free Air Serbia sample response,\
  \ no payment challenge. Not declared in the OpenAPI.\n  - path: /health\n    method: get\n    note: Service health plus dataset snapshot metadata. Not declared in the OpenAPI.\npaid_operations:\n  - operationId: getSerbianCompany\n    price_usd: '0.01'\n  - operationId: searchSerbianCompanies\n    price_usd: '0.01'\n  - operationId: batchGetSerbianCompanies\n    price_usd: '0.05'\ngaps:\n  - >-\n    The OpenAPI has no securitySchemes entry for the payment gate. An x402 scheme is not yet an\n    OpenAPI securityScheme type, but the per-operation x-payment-info extension is present and could\n    be complemented by a documented scheme so spec-only consumers see the 402 contract.\n  - >-\n    The 402 challenge is returned before request validation — an invalid mb or a too-short q also\n    returns 402 rather than 400, so a caller cannot distinguish a malformed request from an unpaid one\n    without paying first.\ncross_links:\n  conventions: conventions/serbia-company-data-conventions.yml\n\
  \  errors: errors/serbia-company-data-problem-types.yml\n  examples: examples/serbia-company-data-402-payment-required.json\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n    - url: https://serbia-company-x402.vercel.app/api/company?mb=07044275\n      http_status: 402\n    - url: https://serbia-company-x402.vercel.app/api/search?q=air%20serbia\n      http_status: 402\n    - url: https://serbia-company-x402.vercel.app/api/company/batch\n      http_status: 402\n    - url: https://serbia-company-x402.vercel.app/api/sample\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/authentication/serbia-company-data-authentication.yml
summary_line: none/x402-payment · 1 scheme
tags:
- serbia
- company-data
- business-registry
- open-data
- x402
- base-usdc
- openapi
- financial-statements
- pay-per-call
- agent-native
---
