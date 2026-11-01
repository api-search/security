---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snaptrade-account-information-api-openapi.yml
  format: yaml
  label: SnapTrade Account Information API
  slug: snaptrade-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-account-information-api-openapi.yml
- filename: snaptrade-api-status-api-openapi.yml
  format: yaml
  label: SnapTrade API Status API
  slug: snaptrade-api-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-api-status-api-openapi.yml
- filename: snaptrade-authentication-api-openapi.yml
  format: yaml
  label: SnapTrade Authentication API
  slug: snaptrade-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-authentication-api-openapi.yml
- filename: snaptrade-connections-api-openapi.yml
  format: yaml
  label: SnapTrade Connections API
  slug: snaptrade-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-connections-api-openapi.yml
- filename: snaptrade-management-api-openapi.yml
  format: yaml
  label: SnapTrade Management API
  slug: snaptrade-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-management-api-openapi.yml
- filename: snaptrade-reference-data-api-openapi.yml
  format: yaml
  label: SnapTrade Reference Data API
  slug: snaptrade-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-reference-data-api-openapi.yml
- filename: snaptrade-trading-api-openapi.yml
  format: yaml
  label: SnapTrade Trading API
  slug: snaptrade-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-trading-api-openapi.yml
auth_types: []
description: SnapTrade uses a Commercial API Key authentication method.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Snaptrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnapTrade declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SnapTrade
provider_slug: snaptrade
scheme_count: 1
schemes:
- evidence: Credentials clientId * consumerKey *
  name: Commercial API Key
  type: other
slug: snaptrade-authentication
source_filename: snaptrade-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.snaptrade.com/reference/Authentication/Authentication_registerSnapTradeUser.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.snaptrade.com/reference/Authentication/Authentication_registerSnapTradeUser.md\nsources:\n- https://docs.snaptrade.com/reference/Authentication/Authentication_registerSnapTradeUser.md\n- https://docs.snaptrade.com/reference/Authentication/Authentication_loginSnapTradeUser.md\n- https://docs.snaptrade.com/reference/Authentication/Authentication_registerSnapTradeUser\n- https://docs.snaptrade.com/reference/Authentication/Authentication_loginSnapTradeUser\ndescription: SnapTrade uses a Commercial API Key authentication method.\nschemes:\n- type: other\n  name: Commercial API Key\n  evidence: Credentials clientId * consumerKey *\nnote: The documentation does not specify the exact placement (header, query, or body) of the clientId and consumerKey, nor does it provide OAuth\n  flow details.\ndocs: https://docs.snaptrade.com/reference/Authentication/Authentication_registerSnapTradeUser.md\n"
source_yaml_url: https://artifacts.apis.io/snaptrade/authentication/snaptrade-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Brokerage
- Trading
---
