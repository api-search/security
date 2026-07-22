---
api_key_in: []
api_specs:
- filename: rift-openapi.yml
  format: yaml
  label: Rift Router API
  slug: rift-router
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rift/refs/heads/main/openapi/rift-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rift declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Rift
provider_slug: rift
scheme_count: 0
schemes: []
slug: rift-authentication
source_filename: rift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rift.trade/api\nsummary:\n  types: []\n  detail: >-\n    Rift's beta Router API reference documents no authentication scheme on any\n    of its four endpoints (/quote, /order/market, /health, /providers). The\n    /health and /providers endpoints are explicitly stated to require no\n    authentication and respond publicly. The quote and order operations define\n    a 401 response, so access may be gated during beta, but no API key, bearer,\n    or OAuth mechanism is published.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rift/refs/heads/main/authentication/rift-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Crypto Defi
- DEX Aggregator
- Cross-Chain
- Trading
- Swaps
- Bridge
- Best Execution
---
