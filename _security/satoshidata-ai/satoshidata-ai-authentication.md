---
anonymous_access: false
api_key_in: []
api_specs:
- filename: satoshidata-ai-batch-api-openapi.yml
  format: yaml
  label: satoshidata-ai Batch API
  slug: satoshidata-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-batch-api-openapi.yml
- filename: satoshidata-ai-billing-api-openapi.yml
  format: yaml
  label: satoshidata-ai Billing API
  slug: satoshidata-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-billing-api-openapi.yml
- filename: satoshidata-ai-chain-api-openapi.yml
  format: yaml
  label: satoshidata-ai Chain API
  slug: satoshidata-ai-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-chain-api-openapi.yml
- filename: satoshidata-ai-community-api-openapi.yml
  format: yaml
  label: satoshidata-ai Community API
  slug: satoshidata-ai-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-community-api-openapi.yml
- filename: satoshidata-ai-discovery-api-openapi.yml
  format: yaml
  label: satoshidata-ai Discovery API
  slug: satoshidata-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-discovery-api-openapi.yml
- filename: satoshidata-ai-entities-api-openapi.yml
  format: yaml
  label: satoshidata-ai Entities API
  slug: satoshidata-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-entities-api-openapi.yml
- filename: satoshidata-ai-feedback-api-openapi.yml
  format: yaml
  label: satoshidata-ai Feedback API
  slug: satoshidata-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-feedback-api-openapi.yml
- filename: satoshidata-ai-health-api-openapi.yml
  format: yaml
  label: satoshidata-ai Health API
  slug: satoshidata-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-health-api-openapi.yml
- filename: satoshidata-ai-labels-api-openapi.yml
  format: yaml
  label: satoshidata-ai Labels API
  slug: satoshidata-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-labels-api-openapi.yml
- filename: satoshidata-ai-market-api-openapi.yml
  format: yaml
  label: satoshidata-ai Market API
  slug: satoshidata-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-market-api-openapi.yml
- filename: satoshidata-ai-metrics-api-openapi.yml
  format: yaml
  label: satoshidata-ai Metrics API
  slug: satoshidata-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-metrics-api-openapi.yml
- filename: satoshidata-ai-risk-api-openapi.yml
  format: yaml
  label: satoshidata-ai Risk API
  slug: satoshidata-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-risk-api-openapi.yml
- filename: satoshidata-ai-sanctions-api-openapi.yml
  format: yaml
  label: satoshidata-ai Sanctions API
  slug: satoshidata-ai-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-sanctions-api-openapi.yml
- filename: satoshidata-ai-timestamping-api-openapi.yml
  format: yaml
  label: satoshidata-ai Timestamping API
  slug: satoshidata-ai-timestamping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-timestamping-api-openapi.yml
- filename: satoshidata-ai-wallets-api-openapi.yml
  format: yaml
  label: satoshidata-ai Wallets API
  slug: satoshidata-ai-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-wallets-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Satoshidata Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: satoshidata-ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: satoshidata-ai
provider_slug: satoshidata-ai
scheme_count: 3
schemes:
- description: Future access model supports this header.
  in: header
  name: X-WR-API-Key
  type: apiKey
- description: Native Lightning L402 authentication.
  name: Lightning L402
  type: l402
- description: USDC on Base token authentication.
  name: x402 USDC on Base
  type: x402
slug: satoshidata-ai-authentication
source_filename: satoshidata-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://satoshidata.ai/docs/\nschemes:\n  - type: apiKey\n    name: X-WR-API-Key\n    in: header\n    description: Future access model supports this header.\n  - type: l402\n    name: Lightning L402\n    description: Native Lightning L402 authentication.\n  - type: x402\n    name: x402 USDC on Base\n    description: USDC on Base token authentication.\n"
source_yaml_url: https://artifacts.apis.io/satoshidata-ai/authentication/satoshidata-ai-authentication.yml
summary_line: 3 schemes
tags:
- Bitcoin
- API
- AI
- Finance
- Chain-Intelligence
- Company
---
