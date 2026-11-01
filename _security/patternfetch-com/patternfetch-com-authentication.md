---
anonymous_access: false
api_key_in: []
api_specs:
- filename: patternfetch-com-api-openapi.json
  format: json
  label: patternfetch Api API
  slug: patternfetch-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/patternfetch-com/openapi/_original/patternfetch-com-api-openapi.json
auth_types: []
description: Authentication for Patternfetch API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Patternfetch Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: patternfetch-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: patternfetch-com
provider_slug: patternfetch-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer pf_…'
  header: Authorization
  how_to_obtain: API key prefixed with pf_ provided after sign‑up
  location: header
  name: Bearer
  type: http-bearer
slug: patternfetch-com-authentication
source_filename: patternfetch-com-authentication.yml
source_heading: Authentication Profile
source_url: https://patternfetch.com/token-cost-study
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://patternfetch.com/token-cost-study\nsources:\n- https://patternfetch.com/token-cost-study\n- https://patternfetch.com/llm-token-cost-ohlcv-candles\n- https://patternfetch.com/market-data-tokens-per-call-benchmark\ndescription: Authentication for Patternfetch API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer pf_…'\n  location: header\n  header: Authorization\n  how_to_obtain: API key prefixed with pf_ provided after sign‑up\ndocs: https://patternfetch.com/token-cost-study\n"
source_yaml_url: https://artifacts.apis.io/patternfetch-com/authentication/patternfetch-com-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- MarketData
- API
- Stocks
- Crypto
---
