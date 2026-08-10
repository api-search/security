---
api_key_in: []
api_specs:
- filename: gleefulai-audit-api-openapi.yml
  format: yaml
  label: Gleeful AI Audit API
  slug: gleefulai-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-audit-api-openapi.yml
- filename: gleefulai-bots-api-openapi.yml
  format: yaml
  label: Gleeful AI Bots API
  slug: gleefulai-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-bots-api-openapi.yml
- filename: gleefulai-capabilities-api-openapi.yml
  format: yaml
  label: Gleeful AI Capabilities API
  slug: gleefulai-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-capabilities-api-openapi.yml
- filename: gleefulai-catalog-api-openapi.yml
  format: yaml
  label: Gleeful AI Catalog API
  slug: gleefulai-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-catalog-api-openapi.yml
- filename: gleefulai-cite-api-openapi.yml
  format: yaml
  label: Gleeful AI Cite API
  slug: gleefulai-cite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-cite-api-openapi.yml
- filename: gleefulai-compare-api-openapi.yml
  format: yaml
  label: Gleeful AI Compare API
  slug: gleefulai-compare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-compare-api-openapi.yml
- filename: gleefulai-content-api-openapi.yml
  format: yaml
  label: Gleeful AI Content API
  slug: gleefulai-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-content-api-openapi.yml
- filename: gleefulai-examples-api-openapi.yml
  format: yaml
  label: Gleeful AI Examples API
  slug: gleefulai-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-examples-api-openapi.yml
- filename: gleefulai-fixes-api-openapi.yml
  format: yaml
  label: Gleeful AI Fixes API
  slug: gleefulai-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-fixes-api-openapi.yml
- filename: gleefulai-health-api-openapi.yml
  format: yaml
  label: Gleeful AI Health API
  slug: gleefulai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-health-api-openapi.yml
- filename: gleefulai-llms-api-openapi.yml
  format: yaml
  label: Gleeful AI Llms API
  slug: gleefulai-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-llms-api-openapi.yml
- filename: gleefulai-meta-api-openapi.yml
  format: yaml
  label: Gleeful AI Meta API
  slug: gleefulai-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-meta-api-openapi.yml
- filename: gleefulai-preview-api-openapi.yml
  format: yaml
  label: Gleeful AI Preview API
  slug: gleefulai-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-preview-api-openapi.yml
- filename: gleefulai-pricing-api-openapi.yml
  format: yaml
  label: Gleeful AI Pricing API
  slug: gleefulai-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-pricing-api-openapi.yml
- filename: gleefulai-probe-api-openapi.yml
  format: yaml
  label: Gleeful AI Probe API
  slug: gleefulai-probe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-probe-api-openapi.yml
- filename: gleefulai-schema-api-openapi.yml
  format: yaml
  label: Gleeful AI Schema API
  slug: gleefulai-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-schema-api-openapi.yml
- filename: gleefulai-status-api-openapi.yml
  format: yaml
  label: Gleeful AI Status API
  slug: gleefulai-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/openapi/gleefulai-status-api-openapi.yml
auth_types: []
description: 'No API keys. Access is priced per call and settled with x402 micropayments — an unauthenticated request returns HTTP 402 with a Payment-Required header carrying a base64 x402 v2 challenge, and the caller pays USDC on Base to proceed. This is a keyless, agent-native access model: an agent can discover the price and pay without a human ever creating an account.'
kind: authentication
layout: security
method: probed
name: Gleefulai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gleeful AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gleeful AI
provider_slug: gleefulai
scheme_count: 1
schemes:
- asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC)
  header: Payment-Required
  id: x402
  max_timeout_seconds: 300
  network: eip155:8453 (Base)
  pay_to: '0x9b916480d6D32c055563cD0B191543E9851F4E2F'
  protocol: x402
  scheme: exact
  type: payment
  version: 2
slug: gleefulai-authentication
source_filename: gleefulai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-03'\nmethod: probed\nstatus: published\nprovider_published: true\nsource: https://visibility.gleefulai.com/openapi.json\ndescription: 'No API keys. Access is priced per call and settled with x402 micropayments\n  — an unauthenticated request returns HTTP 402 with a Payment-Required header carrying\n  a base64 x402 v2 challenge, and the caller pays USDC on Base to proceed. This is\n  a keyless, agent-native access model: an agent can discover the price and pay without\n  a human ever creating an account.'\nverified: '2026-08-03'\nschemes:\n- id: x402\n  type: payment\n  protocol: x402\n  version: 2\n  header: Payment-Required\n  network: eip155:8453 (Base)\n  asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC)\n  pay_to: '0x9b916480d6D32c055563cD0B191543E9851F4E2F'\n  scheme: exact\n  max_timeout_seconds: 300\nkeyless_access:\n  available: true\n  free_endpoints:\n  - /api/health\n  - /api/status\n  - /api/catalog\n  - /api/pricing\n  - /api/capabilities\n\
  \  - /api/preview/audit\n  - /api/preview/compare\n  - /api/examples/{endpoint}\n  note: Discovery, pricing, capabilities and two teaser previews are free and unauthenticated.\nevidence:\n- url: https://visibility.gleefulai.com/api/audit/score\n  status: 402\n  method: POST\n  note: Live 402 confirmed, Payment-Required header carried a decodable x402 v2 challenge.\n- url: https://visibility.gleefulai.com/api/pricing\n  status: 200\n  note: Machine-readable price table, 14 endpoints, USDC on Base.\n- url: https://visibility.gleefulai.com/api/capabilities\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gleefulai/refs/heads/main/authentication/gleefulai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Agents
- x402
- Micropayments
- SEO
- Audit
- Website
- Content
- Crawlers
- Monetization
---
