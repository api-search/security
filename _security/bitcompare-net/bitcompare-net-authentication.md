---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitcompare-net-benchmarks-api-openapi.yml
  format: yaml
  label: Bitcompare Benchmarks API
  slug: bitcompare-net-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-benchmarks-api-openapi.yml
- filename: bitcompare-net-coins-api-openapi.yml
  format: yaml
  label: Bitcompare Coins API
  slug: bitcompare-net-coins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-coins-api-openapi.yml
- filename: bitcompare-net-earn-api-openapi.yml
  format: yaml
  label: Bitcompare Earn API
  slug: bitcompare-net-earn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-earn-api-openapi.yml
- filename: bitcompare-net-market-api-openapi.yml
  format: yaml
  label: Bitcompare Market API
  slug: bitcompare-net-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-market-api-openapi.yml
- filename: bitcompare-net-mcp-api-openapi.yml
  format: yaml
  label: Bitcompare MCP API
  slug: bitcompare-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-mcp-api-openapi.yml
- filename: bitcompare-net-prices-api-openapi.yml
  format: yaml
  label: Bitcompare Prices API
  slug: bitcompare-net-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-prices-api-openapi.yml
- filename: bitcompare-net-rates-api-openapi.yml
  format: yaml
  label: Bitcompare Rates API
  slug: bitcompare-net-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-rates-api-openapi.yml
- filename: bitcompare-net-stablecoins-api-openapi.yml
  format: yaml
  label: Bitcompare Stablecoins API
  slug: bitcompare-net-stablecoins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-stablecoins-api-openapi.yml
- filename: bitcompare-net-symbols-api-openapi.yml
  format: yaml
  label: Bitcompare Symbols API
  slug: bitcompare-net-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-symbols-api-openapi.yml
auth_types: []
description: Authentication methods for Bitcompare API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bitcompare Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitcompare declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bitcompare
provider_slug: bitcompare-net
scheme_count: 1
schemes:
- evidence: Pass your API key as a Bearer token in the Authorization header to unlock higher rate limits and per-key usage tracking.
  header: Authorization
  how_to_obtain: Create and manage keys at the Bitcompare dashboard; keys have a ck_live_ prefix followed by 64 hex characters.
  location: header
  name: API Key
  scopes:
  - rates:read
  - analytics:read
  - clicks:read
  type: http-bearer
slug: bitcompare-net-authentication
source_filename: bitcompare-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bitcompare.net/api-keys
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bitcompare.net/api-keys\nsources:\n- https://docs.bitcompare.net/api-keys\n- https://docs.bitcompare.net/authentication\n- https://docs.bitcompare.net/ad-network/session-tokens\n- https://docs.bitcompare.net/quickstart\ndescription: Authentication methods for Bitcompare API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Pass your API key as a Bearer token in the Authorization header to unlock higher rate limits and per-key usage tracking.\n  location: header\n  header: Authorization\n  scopes:\n  - rates:read\n  - analytics:read\n  - clicks:read\n  how_to_obtain: Create and manage keys at the Bitcompare dashboard; keys have a ck_live_ prefix followed by 64 hex characters.\ndocs: https://docs.bitcompare.net/api-keys\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/bitcompare-net/authentication/bitcompare-net-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Finance
- Data
- Yield
---
