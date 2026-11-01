---
anonymous_access: false
api_key_in: []
api_specs:
- filename: birdeye-so-data-openapi-generated.yml
  format: yaml
  label: Birdeye (Solana data) data API
  slug: data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdeye-so/openapi/_ae-authored/birdeye-so-data-openapi-generated.yml
- filename: birdeye-so-resources-openapi-generated.yml
  format: yaml
  label: Birdeye (Solana data) resources API
  slug: resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdeye-so/openapi/_ae-authored/birdeye-so-resources-openapi-generated.yml
auth_types: []
description: Birdeye APIs use API‑key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Birdeye So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Birdeye (Solana data) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Birdeye (Solana data)
provider_slug: birdeye-so
scheme_count: 1
schemes:
- evidence: Birdeye APIs use API-key authentication.
  header: X-API-KEY
  how_to_obtain: Generate a key in the Security tab of the dashboard.
  location: header
  name: X-API-KEY
  type: apiKey
slug: birdeye-so-authentication
source_filename: birdeye-so-authentication.yml
source_heading: Authentication Profile
source_url: https://data.birdeye.so/docs/authentication
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://data.birdeye.so/docs/authentication\nsources:\n- https://data.birdeye.so/docs/authentication\n- https://data.birdeye.so/docs/data-api/price-ohlcv/get-defi-v3-liquidity-ohlc-token\n- https://data.birdeye.so/docs/data-api/price-ohlcv/get-defi-v3-liquidity-history-token\n- https://data.birdeye.so/docs/data-api/price-ohlcv/post-defi-v3-liquidity-latest-token\ndescription: Birdeye APIs use API‑key authentication.\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: Birdeye APIs use API-key authentication.\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Generate a key in the Security tab of the dashboard.\nnote: No OAuth or other authentication methods are documented.\ndocs: https://data.birdeye.so/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/birdeye-so/authentication/birdeye-so-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Blockchain
- Data
- Analytics
- Token
---
