---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magicmarkets-com-account-api-openapi.yml
  format: yaml
  label: MagicMarkets Account API
  slug: magicmarkets-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-account-api-openapi.yml
- filename: magicmarkets-com-betslips-api-openapi.yml
  format: yaml
  label: MagicMarkets Betslips API
  slug: magicmarkets-com-betslips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-betslips-api-openapi.yml
- filename: magicmarkets-com-heartbeats-api-openapi.yml
  format: yaml
  label: MagicMarkets Heartbeats API
  slug: magicmarkets-com-heartbeats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-heartbeats-api-openapi.yml
- filename: magicmarkets-com-market-data-api-openapi.yml
  format: yaml
  label: MagicMarkets Market data API
  slug: magicmarkets-com-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-market-data-api-openapi.yml
- filename: magicmarkets-com-orders-api-openapi.yml
  format: yaml
  label: MagicMarkets Orders API
  slug: magicmarkets-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-orders-api-openapi.yml
- filename: magicmarkets-com-reference-api-openapi.yml
  format: yaml
  label: MagicMarkets Reference API
  slug: magicmarkets-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-reference-api-openapi.yml
- filename: magicmarkets-com-streaming-api-api-openapi.yml
  format: yaml
  label: MagicMarkets Streaming API
  slug: magicmarkets-com-streaming-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicmarkets-com/openapi/magicmarkets-com-streaming-api-api-openapi.yml
auth_types: []
description: Authentication for MagicMarkets API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MagicMarkets Authentication
name_suffix: Authentication
oauth_flows: []
overview: MagicMarkets declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MagicMarkets
provider_slug: magicmarkets-com
scheme_count: 2
schemes:
- evidence: Send the key in the `X-Api-Key` header on every request.
  header: X-Api-Key
  how_to_obtain: Create an API key in the website Settings → API page; the key is shown once at creation.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: A handshake cannot carry a header, so the key goes in the query string.
  how_to_obtain: Create an API key in the website Settings → API page; the key is shown once at creation.
  location: query
  name: api_key
  type: apiKey
slug: magicmarkets-com-authentication
source_filename: magicmarkets-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.magicmarkets.com/developers/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.magicmarkets.com/developers/authentication.md\nsources:\n- https://docs.magicmarkets.com/developers/authentication.md\n- https://docs.magicmarkets.com/traders/getting-started/create-account.md\n- https://docs.magicmarkets.com/traders/getting-started/first-deposit.md\n- https://docs.magicmarkets.com/traders/getting-started/first-trade.md\ndescription: Authentication for MagicMarkets API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: Send the key in the `X-Api-Key` header on every request.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create an API key in the website Settings → API page; the key is shown once at creation.\n- type: apiKey\n  name: api_key\n  evidence: A handshake cannot carry a header, so the key goes in the query string.\n  location: query\n  how_to_obtain: Create an API key in the website Settings → API page; the key is shown\
  \ once at creation.\nnote: The public API uses only API keys; no other authentication methods are documented.\ndocs: https://docs.magicmarkets.com/developers/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/magicmarkets-com/authentication/magicmarkets-com-authentication.yml
summary_line: 2 schemes
tags:
- Sports
- Prediction-Market
- Trading
- Finance
- Costa-Rica
---
