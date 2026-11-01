---
anonymous_access: false
api_key_in: []
api_specs:
- filename: polystrike-xyz-bulk-api-openapi.yml
  format: yaml
  label: polystrike-xyz Bulk API
  slug: polystrike-xyz-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-bulk-api-openapi.yml
- filename: polystrike-xyz-history-api-openapi.yml
  format: yaml
  label: polystrike-xyz History API
  slug: polystrike-xyz-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-history-api-openapi.yml
- filename: polystrike-xyz-metadata-api-openapi.yml
  format: yaml
  label: polystrike-xyz Metadata API
  slug: polystrike-xyz-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-metadata-api-openapi.yml
- filename: polystrike-xyz-performance-api-openapi.yml
  format: yaml
  label: polystrike-xyz Performance API
  slug: polystrike-xyz-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-performance-api-openapi.yml
- filename: polystrike-xyz-portfolio-api-openapi.yml
  format: yaml
  label: polystrike-xyz Portfolio API
  slug: polystrike-xyz-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-portfolio-api-openapi.yml
- filename: polystrike-xyz-predictions-api-openapi.yml
  format: yaml
  label: polystrike-xyz Predictions API
  slug: polystrike-xyz-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-predictions-api-openapi.yml
- filename: polystrike-xyz-signals-api-openapi.yml
  format: yaml
  label: polystrike-xyz Signals API
  slug: polystrike-xyz-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-signals-api-openapi.yml
- filename: polystrike-xyz-system-api-openapi.yml
  format: yaml
  label: polystrike-xyz System API
  slug: polystrike-xyz-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-system-api-openapi.yml
- filename: polystrike-xyz-usage-api-openapi.yml
  format: yaml
  label: polystrike-xyz Usage API
  slug: polystrike-xyz-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Polystrike Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: polystrike-xyz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: polystrike-xyz
provider_slug: polystrike-xyz
scheme_count: 2
schemes:
- description: API key for authentication. Get yours at https://polystrike.xyz
  in: header
  name: X-API-Key
  type: apiKey
- description: Coinbase payment protocol for per-call payments
  in: header
  name: x402
  type: apiKey
slug: polystrike-xyz-authentication
source_filename: polystrike-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://polystrike.xyz/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key for authentication. Get yours at https://polystrike.xyz\n  - type: apiKey\n    name: x402\n    in: header\n    description: Coinbase payment protocol for per-call payments\n"
source_yaml_url: https://artifacts.apis.io/polystrike-xyz/authentication/polystrike-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- Prediction-Market
- API
- Crypto
---
