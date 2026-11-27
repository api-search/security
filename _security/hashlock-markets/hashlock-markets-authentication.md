---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hashlock-markets-assets-api-openapi.yml
  format: yaml
  label: Hashlock Markets Assets API
  slug: hashlock-markets-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-assets-api-openapi.yml
- filename: hashlock-markets-keys-api-openapi.yml
  format: yaml
  label: Hashlock Markets Keys API
  slug: hashlock-markets-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-keys-api-openapi.yml
- filename: hashlock-markets-me-api-openapi.yml
  format: yaml
  label: Hashlock Markets Me API
  slug: hashlock-markets-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-me-api-openapi.yml
- filename: hashlock-markets-rfqs-api-openapi.yml
  format: yaml
  label: Hashlock Markets Rfqs API
  slug: hashlock-markets-rfqs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-rfqs-api-openapi.yml
- filename: hashlock-markets-swaps-api-openapi.yml
  format: yaml
  label: Hashlock Markets Swaps API
  slug: hashlock-markets-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-swaps-api-openapi.yml
- filename: hashlock-markets-threads-api-openapi.yml
  format: yaml
  label: Hashlock Markets Threads API
  slug: hashlock-markets-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-threads-api-openapi.yml
- filename: hashlock-markets-tx-api-openapi.yml
  format: yaml
  label: Hashlock Markets Tx API
  slug: hashlock-markets-tx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-tx-api-openapi.yml
- filename: hashlock-markets-wallets-api-openapi.yml
  format: yaml
  label: Hashlock Markets Wallets API
  slug: hashlock-markets-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-wallets-api-openapi.yml
- filename: hashlock-markets-webhooks-api-openapi.yml
  format: yaml
  label: Hashlock Markets Webhooks API
  slug: hashlock-markets-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-webhooks-api-openapi.yml
auth_types: []
description: Authentication uses API keys.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hashlock Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hashlock Markets declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hashlock Markets
provider_slug: hashlock-markets
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer hk_live_...'
  header: Authorization
  location: header
  name: Authorization header Bearer token
  type: apiKey
- evidence: 'X-Api-Key: hk_live_...'
  header: X-Api-Key
  location: header
  name: X-Api-Key header
  type: apiKey
slug: hashlock-markets-authentication
source_filename: hashlock-markets-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hashlock.markets/guides/api-keys.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hashlock.markets/guides/api-keys.md\nsources:\n- https://docs.hashlock.markets/guides/api-keys.md\n- https://docs.hashlock.markets/api-reference/start-minting-an-api-key:-a-single-use-nonce-5-minutes-no-key-needed.md\n- https://docs.hashlock.markets/guides/token-listing.md\ndescription: Authentication uses API keys.\nschemes:\n- type: apiKey\n  name: Authorization header Bearer token\n  evidence: 'Authorization: Bearer hk_live_...'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-Api-Key header\n  evidence: 'X-Api-Key: hk_live_...'\n  location: header\n  header: X-Api-Key\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://docs.hashlock.markets/guides/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/hashlock-markets/authentication/hashlock-markets-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Cryptocurrency
- AtomicSwap
- Non-Custodial
- Cross-Chain
---
