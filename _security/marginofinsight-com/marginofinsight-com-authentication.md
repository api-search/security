---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: marginofinsight-com-account-api-openapi.yml
  format: yaml
  label: Margin of Insight Account API
  slug: marginofinsight-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginofinsight-com/openapi/marginofinsight-com-account-api-openapi.yml
- filename: marginofinsight-com-coverage-api-openapi.yml
  format: yaml
  label: Margin of Insight Coverage API
  slug: marginofinsight-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginofinsight-com/openapi/marginofinsight-com-coverage-api-openapi.yml
- filename: marginofinsight-com-research-api-openapi.yml
  format: yaml
  label: Margin of Insight Research API
  slug: marginofinsight-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginofinsight-com/openapi/marginofinsight-com-research-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Margin of Insight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Margin of Insight secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Margin of Insight
provider_slug: marginofinsight-com
scheme_count: 2
schemes:
- bearerFormat: spt_…
  description: 'Stripe Link Shared Payment Token (SPT). Your operator authorizes you in Stripe Link with a max_amount scoped to marginofinsight''s network_business_profile; pass the resulting `spt_…` token as `Authorization: Bearer spt_…`. The token is introspected and charged per call via Stripe — no marginofinsight account, no pre-funded balance, no static credential. Discovery: GET /api/v1/well-known/spt. See h'
  name: StripeSpt
  scheme: bearer
  sources:
  - openapi/marginofinsight-com-openapi.json
  type: http
- description: 'Autonomous agent payment via x402 protocol (HTTP 402 + USDC on Base). Planned (Phase 5, not yet live). Once shipped: call the endpoint without auth; server returns 402 with payment terms; sign and retry.'
  in: header
  name: x402
  parameter: X-Payment
  sources:
  - openapi/marginofinsight-com-openapi.json
  type: apiKey
slug: marginofinsight-com-authentication
source_filename: marginofinsight-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/marginofinsight-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: StripeSpt\n  type: http\n  scheme: bearer\n  bearerFormat: spt_…\n  description: 'Stripe Link Shared Payment Token (SPT). Your operator authorizes you in Stripe\n    Link with a max_amount scoped to marginofinsight''s network_business_profile; pass the resulting\n    `spt_…` token as `Authorization: Bearer spt_…`. The token is introspected and charged per\n    call via Stripe — no marginofinsight account, no pre-funded balance, no static credential.\n    Discovery: GET /api/v1/well-known/spt. See h'\n  sources:\n  - openapi/marginofinsight-com-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-Payment\n  description: 'Autonomous agent payment via x402 protocol (HTTP 402 + USDC on Base). Planned\n    (Phase 5, not yet live). Once shipped: call the endpoint without auth; server\
  \ returns 402\n    with payment terms; sign and retry.'\n  sources:\n  - openapi/marginofinsight-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/marginofinsight-com/authentication/marginofinsight-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Equity Research
- Financial Data
- AI Agents
- US‑Listed SEC Filers
---
