---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gammaflip-io-data-api-openapi.yml
  format: yaml
  label: GammaFlip.io Data API
  slug: gammaflip-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-data-api-openapi.yml
- filename: gammaflip-io-discovery-api-openapi.yml
  format: yaml
  label: GammaFlip.io Discovery API
  slug: gammaflip-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-discovery-api-openapi.yml
- filename: gammaflip-io-history-api-openapi.yml
  format: yaml
  label: GammaFlip.io History API
  slug: gammaflip-io-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-history-api-openapi.yml
auth_types: []
description: Authentication methods for GammaFlip.io API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GammaFlip.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: GammaFlip.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GammaFlip.io
provider_slug: gammaflip-io
scheme_count: 1
schemes:
- evidence: 'Include the key in the `X-API-Key` HTTP header on every request:'
  header: X-API-Key
  how_to_obtain: Keys are generated at https://gammaflip.io/account and shown only once at creation.
  location: header
  name: API Key
  type: apiKey
slug: gammaflip-io-authentication
source_filename: gammaflip-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.gammaflip.io/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.gammaflip.io/authentication.md\nsources:\n- https://docs.gammaflip.io/authentication.md\n- https://docs.gammaflip.io/quickstart.md\ndescription: Authentication methods for GammaFlip.io API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include the key in the `X-API-Key` HTTP header on every request:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Keys are generated at https://gammaflip.io/account and shown only once at creation.\ndocs: https://docs.gammaflip.io/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/gammaflip-io/authentication/gammaflip-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Cryptocurrency
- Market Data
- Trading
---
