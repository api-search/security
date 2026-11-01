---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quantsonar-com-default-api-openapi.yml
  format: yaml
  label: quantsonar-com 分红送股 API
  slug: quantsonar-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-default-api-openapi.yml
- filename: quantsonar-com-etf-api-openapi.yml
  format: yaml
  label: quantsonar-com ETF API
  slug: quantsonar-com-etf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-etf-api-openapi.yml
- filename: quantsonar-com-health-api-openapi.yml
  format: yaml
  label: quantsonar-com Health API
  slug: quantsonar-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-health-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Quantsonar Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: quantsonar-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: quantsonar-com
provider_slug: quantsonar-com
scheme_count: 1
schemes:
- description: API key provided in the console, sent as X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: quantsonar-com-authentication
source_filename: quantsonar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://quantsonar.com/en/docs#auth\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key provided in the console, sent as X-API-Key header.\n"
source_yaml_url: https://artifacts.apis.io/quantsonar-com/authentication/quantsonar-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Data
- API
- China
- Stock-Market
---
