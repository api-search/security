---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commonrig-com-a2a-api-openapi.yml
  format: yaml
  label: CommonRig A2a API
  slug: commonrig-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-a2a-api-openapi.yml
- filename: commonrig-com-beacon-api-openapi.yml
  format: yaml
  label: CommonRig Beacon API
  slug: commonrig-com-beacon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-beacon-api-openapi.yml
- filename: commonrig-com-buy-api-openapi.yml
  format: yaml
  label: CommonRig Buy API
  slug: commonrig-com-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-buy-api-openapi.yml
- filename: commonrig-com-check-api-openapi.yml
  format: yaml
  label: CommonRig Check API
  slug: commonrig-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-check-api-openapi.yml
- filename: commonrig-com-checkout-api-openapi.yml
  format: yaml
  label: CommonRig Checkout API
  slug: commonrig-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-checkout-api-openapi.yml
- filename: commonrig-com-commonrig-store-api-openapi.yml
  format: yaml
  label: CommonRig CommonRig Store API
  slug: commonrig-com-commonrig-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-commonrig-store-api-openapi.yml
- filename: commonrig-com-doctor-api-openapi.yml
  format: yaml
  label: CommonRig Doctor API
  slug: commonrig-com-doctor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-doctor-api-openapi.yml
- filename: commonrig-com-kit-api-openapi.yml
  format: yaml
  label: CommonRig Kit API
  slug: commonrig-com-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-kit-api-openapi.yml
- filename: commonrig-com-licence-api-openapi.yml
  format: yaml
  label: CommonRig Licence API
  slug: commonrig-com-licence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-licence-api-openapi.yml
- filename: commonrig-com-sample-api-openapi.yml
  format: yaml
  label: CommonRig Sample API
  slug: commonrig-com-sample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-sample-api-openapi.yml
- filename: commonrig-com-score-api-openapi.yml
  format: yaml
  label: CommonRig Score API
  slug: commonrig-com-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-score-api-openapi.yml
- filename: commonrig-com-stats-api-openapi.yml
  format: yaml
  label: CommonRig Stats API
  slug: commonrig-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-stats-api-openapi.yml
- filename: commonrig-com-updates-api-openapi.yml
  format: yaml
  label: CommonRig Updates API
  slug: commonrig-com-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonrig-com/openapi/commonrig-com-updates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CommonRig Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommonRig secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CommonRig
provider_slug: commonrig-com
scheme_count: 3
schemes:
- applies_to:
  - POST /v1/doctor/check
  - GET /v1/updates
  - GET /v1/updates/packs/{version}
  description: 'The licence key in the receipt is the only credential. Send it as Authorization: Bearer <key> to https://commonrig.com/v1/doctor/check and https://commonrig.com/v1/updates.'
  name: licence
  scheme: bearer
  sources:
  - openapi/commonrig-com-openapi.yml
  - https://commonrig.com/auth.md
  type: http
- applies_to:
  - GET /v1/stats
  description: Bearer token required by GET /v1/stats (aggregated research statistics); how it is issued is not documented publicly.
  name: statsToken
  scheme: bearer
  sources:
  - openapi/commonrig-com-openapi.yml
  type: http
- applies_to:
  - GET /v1/buy/x402
  - POST /v1/check
  description: 'Unauthenticated pay-per-request: GET /v1/buy/x402 and POST /v1/check answer 402 with payment terms and settle in USDC on Base (x402). Everything else is public.'
  name: x402
  sources:
  - openapi/commonrig-com-openapi.yml
  - https://commonrig.com/llms-full.txt
  type: payment
slug: commonrig-com-authentication
source_filename: commonrig-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commonrig.com/auth.md\ndocs: https://commonrig.com/auth.md\nsummary:\n  types:\n  - http\n  note: \"No registration, accounts or OAuth. Per auth.md: \\\"CommonRig has no registration, no accounts and no agent identity flow.\\\" The licence key from the purchase receipt is the only customer credential.\"\nschemes:\n- name: licence\n  type: http\n  scheme: bearer\n  description: \"The licence key in the receipt is the only credential. Send it as Authorization: Bearer <key> to https://commonrig.com/v1/doctor/check and https://commonrig.com/v1/updates.\"\n  applies_to:\n  - POST /v1/doctor/check\n  - GET /v1/updates\n  - GET /v1/updates/packs/{version}\n  sources:\n  - openapi/commonrig-com-openapi.yml\n  - https://commonrig.com/auth.md\n- name: statsToken\n  type: http\n  scheme: bearer\n  description: Bearer token required by GET /v1/stats (aggregated research statistics); how it is issued is not documented publicly.\n\
  \  applies_to:\n  - GET /v1/stats\n  sources:\n  - openapi/commonrig-com-openapi.yml\n- name: x402\n  type: payment\n  description: \"Unauthenticated pay-per-request: GET /v1/buy/x402 and POST /v1/check answer 402 with payment terms and settle in USDC on Base (x402). Everything else is public.\"\n  applies_to:\n  - GET /v1/buy/x402\n  - POST /v1/check\n  sources:\n  - openapi/commonrig-com-openapi.yml\n  - https://commonrig.com/llms-full.txt\n"
source_yaml_url: https://artifacts.apis.io/commonrig-com/authentication/commonrig-com-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- AI Agents
- Claude Code
- Codex
- Developer Tools
- Agent Rules
- Agent Skills
- Coding Agents
- x402
---
