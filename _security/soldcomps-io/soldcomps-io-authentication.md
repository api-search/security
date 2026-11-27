---
anonymous_access: false
api_key_in: []
api_specs:
- filename: soldcomps-io-account-api-openapi.yml
  format: yaml
  label: SoldComps.io Account API
  slug: soldcomps-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldcomps-io/openapi/soldcomps-io-account-api-openapi.yml
- filename: soldcomps-io-sold-comps-api-openapi.yml
  format: yaml
  label: SoldComps.io Sold comps API
  slug: soldcomps-io-sold-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldcomps-io/openapi/soldcomps-io-sold-comps-api-openapi.yml
auth_types: []
description: 'Authentication is done by adding an Authorization: Bearer header with your SoldComps API key.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: SoldComps.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: SoldComps.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SoldComps.io
provider_slug: soldcomps-io
scheme_count: 1
schemes:
- evidence: 'add an Authorization: Bearer header with your SoldComps key for more.'
  header: Authorization
  how_to_obtain: Get a free API key at https://www.soldcomps.io/signup.
  location: header
  name: Bearer
  type: http-bearer
slug: soldcomps-io-authentication
source_filename: soldcomps-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.soldcomps.io/blog/claude-ebay-sold-prices.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.soldcomps.io/blog/claude-ebay-sold-prices.md\nsources:\n- https://www.soldcomps.io/blog/claude-ebay-sold-prices.md\ndescription: 'Authentication is done by adding an Authorization: Bearer header with your SoldComps API key.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'add an Authorization: Bearer header with your SoldComps key for more.'\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free API key at https://www.soldcomps.io/signup.\ndocs: https://www.soldcomps.io/blog/claude-ebay-sold-prices.md\n"
source_yaml_url: https://artifacts.apis.io/soldcomps-io/authentication/soldcomps-io-authentication.yml
summary_line: 1 scheme
tags:
- eBay
- Pricing
- Data
- Marketplace
---
