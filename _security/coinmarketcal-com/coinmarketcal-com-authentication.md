---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coinmarketcal-com-openapi-generated.yml
  format: yaml
  label: CoinMarketCal API
  slug: coinmarketcal-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmarketcal-com/openapi/_ae-authored/coinmarketcal-com-openapi-generated.yml
auth_types: []
description: API-key authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CoinMarketCal Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinMarketCal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoinMarketCal
provider_slug: coinmarketcal-com
scheme_count: 1
schemes:
- evidence: The API uses API-key authentication. Send your key in the x-api-key header on every request.
  header: x-api-key
  how_to_obtain: Open the dashboard, click + New API key and copy the full secret once.
  location: header
  name: x-api-key
  type: apiKey
slug: coinmarketcal-com-authentication
source_filename: coinmarketcal-com-authentication.yml
source_heading: Authentication Profile
source_url: https://coinmarketcal.com/developer/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://coinmarketcal.com/developer/docs/authentication\nsources:\n- https://coinmarketcal.com/developer/docs/authentication\n- https://coinmarketcal.com/developer/docs\ndescription: API-key authentication\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: The API uses API-key authentication. Send your key in the x-api-key header on every request.\n  location: header\n  header: x-api-key\n  how_to_obtain: Open the dashboard, click + New API key and copy the full secret once.\ndocs: https://coinmarketcal.com/developer/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/coinmarketcal-com/authentication/coinmarketcal-com-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Event
- Calendar
- Data
---
