---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outcometick-com-backtest-api-openapi.yml
  format: yaml
  label: Outcometick Backtest API
  slug: outcometick-com-backtest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-backtest-api-openapi.yml
- filename: outcometick-com-data-api-openapi.yml
  format: yaml
  label: Outcometick Data API
  slug: outcometick-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-data-api-openapi.yml
- filename: outcometick-com-public-api-openapi.yml
  format: yaml
  label: Outcometick Public API
  slug: outcometick-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-public-api-openapi.yml
- filename: outcometick-com-purchase-api-openapi.yml
  format: yaml
  label: Outcometick Purchase API
  slug: outcometick-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-purchase-api-openapi.yml
- filename: outcometick-com-smart-money-api-openapi.yml
  format: yaml
  label: Outcometick Smart Money API
  slug: outcometick-com-smart-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-smart-money-api-openapi.yml
auth_types: []
description: Authentication is performed by sending the key as a Bearer token in the Authorization header, or alternatively as an api_key query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Outcometick Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outcometick declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Outcometick
provider_slug: outcometick-com
scheme_count: 1
schemes:
- evidence: 'curl -s -H "Authorization: Bearer $OT_KEY " \ https://outcometick.com/v1/meta'
  header: Authorization
  how_to_obtain: Key is shown once on the payment page after purchase.
  location: header
  name: Bearer
  type: http-bearer
slug: outcometick-com-authentication
source_filename: outcometick-com-authentication.yml
source_heading: Authentication Profile
source_url: https://outcometick.com/docs
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://outcometick.com/docs\nsources:\n- https://outcometick.com/docs\ndescription: Authentication is performed by sending the key as a Bearer token in the Authorization header, or alternatively as an api_key query\n  parameter.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -s -H \"Authorization: Bearer $OT_KEY \" \\ https://outcometick.com/v1/meta'\n  location: header\n  header: Authorization\n  how_to_obtain: Key is shown once on the payment page after purchase.\ndocs: https://outcometick.com/docs\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/outcometick-com/authentication/outcometick-com-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Finance
- Cryptocurrency
- Market Data
---
