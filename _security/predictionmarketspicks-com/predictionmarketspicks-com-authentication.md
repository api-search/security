---
anonymous_access: false
api_key_in: []
api_specs:
- filename: predictionmarketspicks-com-openapi-generated.yml
  format: yaml
  label: predictionmarketspicks-com API
  slug: predictionmarketspicks-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/predictionmarketspicks-com/openapi/_ae-authored/predictionmarketspicks-com-openapi-generated.yml
auth_types: []
description: Authentication is optional; free tools require no credentials, while Pro tools use a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Predictionmarketspicks Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: predictionmarketspicks-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: predictionmarketspicks-com
provider_slug: predictionmarketspicks-com
scheme_count: 1
schemes:
- evidence: 'Adding a Pro key (optional) Pro tools take a PredictionMarketsPicks key as an Authorization: Bearer header on the same server URL.'
  header: Authorization
  how_to_obtain: 'Provision a key at checkout (live at /account/keys) and include it as "Authorization: Bearer <key>".'
  location: header
  name: Bearer
  type: http-bearer
slug: predictionmarketspicks-com-authentication
source_filename: predictionmarketspicks-com-authentication.yml
source_heading: Authentication Profile
source_url: https://predictionmarketspicks.com/mcp/setup
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://predictionmarketspicks.com/mcp/setup\nsources:\n- https://predictionmarketspicks.com/mcp/setup\ndescription: Authentication is optional; free tools require no credentials, while Pro tools use a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Adding a Pro key (optional) Pro tools take a PredictionMarketsPicks key as an Authorization: Bearer header on the same server URL.'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Provision a key at checkout (live at /account/keys) and include it as \"Authorization: Bearer <key>\".'\nnote: Free tools do not require any authentication.\ndocs: https://predictionmarketspicks.com/mcp/setup\n"
source_yaml_url: https://artifacts.apis.io/predictionmarketspicks-com/authentication/predictionmarketspicks-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- PredictionMarkets
- TradingTools
- Analytics
- News
---
