---
anonymous_access: false
api_key_in: []
api_specs:
- filename: atlasyield-club-basket-api-openapi.yml
  format: yaml
  label: AtlasYield Basket API
  slug: atlasyield-club-basket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-basket-api-openapi.yml
- filename: atlasyield-club-catalog-api-openapi.yml
  format: yaml
  label: AtlasYield Catalog API
  slug: atlasyield-club-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-catalog-api-openapi.yml
- filename: atlasyield-club-gas-api-openapi.yml
  format: yaml
  label: AtlasYield Gas API
  slug: atlasyield-club-gas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-gas-api-openapi.yml
- filename: atlasyield-club-portfolio-api-openapi.yml
  format: yaml
  label: AtlasYield Portfolio API
  slug: atlasyield-club-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-portfolio-api-openapi.yml
- filename: atlasyield-club-scores-api-openapi.yml
  format: yaml
  label: AtlasYield Scores API
  slug: atlasyield-club-scores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-scores-api-openapi.yml
- filename: atlasyield-club-vaults-api-openapi.yml
  format: yaml
  label: AtlasYield Vaults API
  slug: atlasyield-club-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-vaults-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Atlasyield Club Authentication
name_suffix: Authentication
oauth_flows: []
overview: AtlasYield declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AtlasYield
provider_slug: atlasyield-club
scheme_count: 1
schemes:
- description: Optional partner key to increase rate limits and unlock partner endpoints. Not required for public endpoints.
  in: header
  name: x-api-key
  type: apiKey
slug: atlasyield-club-authentication
source_filename: atlasyield-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://docs.atlasyield.club/api-reference/introduction.md\nschemes:\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: \"Optional partner key to increase rate limits and unlock partner endpoints. Not required for public endpoints.\"\n"
source_yaml_url: https://artifacts.apis.io/atlasyield-club/authentication/atlasyield-club-authentication.yml
summary_line: 1 scheme
tags:
- DeFi
- Yield
- Risk Management
- Analytics
- Onchain
---
