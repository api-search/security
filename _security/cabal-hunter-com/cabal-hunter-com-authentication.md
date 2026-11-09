---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cabal-hunter-com-cex-funding-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Cex Funding API
  slug: cabal-hunter-com-cex-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-cex-funding-api-openapi.yml
- filename: cabal-hunter-com-cohorts-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Cohorts API
  slug: cabal-hunter-com-cohorts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-cohorts-api-openapi.yml
- filename: cabal-hunter-com-info-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Info API
  slug: cabal-hunter-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-info-api-openapi.yml
- filename: cabal-hunter-com-scan-batch-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Scan Batch API
  slug: cabal-hunter-com-scan-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-scan-batch-api-openapi.yml
- filename: cabal-hunter-com-scan-cabal-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Scan Cabal API
  slug: cabal-hunter-com-scan-cabal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-scan-cabal-api-openapi.yml
- filename: cabal-hunter-com-screen-list-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Screen List API
  slug: cabal-hunter-com-screen-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-screen-list-api-openapi.yml
- filename: cabal-hunter-com-trade-analysis-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Trade Analysis API
  slug: cabal-hunter-com-trade-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-trade-analysis-api-openapi.yml
- filename: cabal-hunter-com-wallet-check-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Wallet Check API
  slug: cabal-hunter-com-wallet-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-wallet-check-api-openapi.yml
- filename: cabal-hunter-com-wallet-report-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Wallet Report API
  slug: cabal-hunter-com-wallet-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-wallet-report-api-openapi.yml
- filename: cabal-hunter-com-watch-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Watch API
  slug: cabal-hunter-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-watch-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Cabal Hunter Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cabal-Hunter secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cabal-Hunter
provider_slug: cabal-hunter-com
scheme_count: 2
schemes:
- description: Your Cabal-Hunter key. Required for watch endpoints so a watch belongs to exactly one caller.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/cabal-hunter-com-openapi.json
  type: apiKey
- description: Solana USDC payment tx signature (x402). Omit for the 5 anonymous scans/month, or use a free key (one email) for 250/month per IP.
  in: header
  name: x402Payment
  parameter: X-Payment-Signature
  sources:
  - openapi/cabal-hunter-com-openapi.json
  type: apiKey
slug: cabal-hunter-com-authentication
source_filename: cabal-hunter-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/cabal-hunter-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your Cabal-Hunter key. Required for watch endpoints so a watch belongs to exactly\n    one caller.\n  sources:\n  - openapi/cabal-hunter-com-openapi.json\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-Payment-Signature\n  description: Solana USDC payment tx signature (x402). Omit for the 5 anonymous scans/month,\n    or use a free key (one email) for 250/month per IP.\n  sources:\n  - openapi/cabal-hunter-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cabal-hunter-com/authentication/cabal-hunter-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Solana
- Cryptocurrency
- Security
- Analytics
---
