---
anonymous_access: false
api_key_in: []
api_specs:
- filename: epsilon-exchange-api-openapi.json
  format: json
  label: Epsilon Public API API
  slug: epsilon-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epsilon-exchange/openapi/_original/epsilon-exchange-api-openapi.json
auth_types: []
description: Epsilon uses a developer API key (eps_…) for authentication. The key can be sent either as an API key header or as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Epsilon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epsilon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Epsilon
provider_slug: epsilon-exchange
scheme_count: 1
schemes:
- evidence: 'Every keyed endpoint accepts the key in either header form: X-API-Key: eps_YOUR_KEY'
  header: X-API-Key
  how_to_obtain: Get an API key. Keys are issued per Epsilon account. During early access, keys are concierge‑issued — ask in the community or DM @TradeEpsilon.
  location: header
  name: X-API-Key
  type: apiKey
slug: epsilon-exchange-authentication
source_filename: epsilon-exchange-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.epsilon.exchange/
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.epsilon.exchange/\nsources:\n- https://developers.epsilon.exchange/\n- https://developers.epsilon.exchange/api/#GET/v1/order-preflight\n- https://developers.epsilon.exchange/api/\ndescription: Epsilon uses a developer API key (eps_…) for authentication. The key can be sent either as an API key header or as a Bearer token.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Every keyed endpoint accepts the key in either header form: X-API-Key: eps_YOUR_KEY'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get an API key. Keys are issued per Epsilon account. During early access, keys are concierge‑issued — ask in the community or\n    DM @TradeEpsilon.\nnote: No OAuth2 flows are documented. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://developers.epsilon.exchange/\n"
source_yaml_url: https://artifacts.apis.io/epsilon-exchange/authentication/epsilon-exchange-authentication.yml
summary_line: 1 scheme
tags:
- Trading
- DeFi
- Cryptocurrency
- AdvancedOrders
- Robinhood Chain
---
