---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ashareapi-com-free-api-openapi.yml
  format: yaml
  label: ashareapi-com Free API
  slug: ashareapi-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ashareapi-com/openapi/ashareapi-com-free-api-openapi.yml
- filename: ashareapi-com-market-kline-api-openapi.yml
  format: yaml
  label: ashareapi-com Market Kline API
  slug: ashareapi-com-market-kline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ashareapi-com/openapi/ashareapi-com-market-kline-api-openapi.yml
- filename: ashareapi-com-pro-api-openapi.yml
  format: yaml
  label: ashareapi-com Pro API
  slug: ashareapi-com-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ashareapi-com/openapi/ashareapi-com-pro-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ashareapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ashareapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ashareapi-com
provider_slug: ashareapi-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Authorization header with Bearer token (API Key)
  scheme: bearer
  type: http
- description: API Key passed as query parameter
  in: query
  name: key
  type: apiKey
slug: ashareapi-com-authentication
source_filename: ashareapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://ashareapi.com/docs/\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Authorization header with Bearer token (API Key)\"\n  - type: apiKey\n    in: query\n    name: key\n    description: \"API Key passed as query parameter\"\n"
source_yaml_url: https://artifacts.apis.io/ashareapi-com/authentication/ashareapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Stock-Market
- Data-API
- China
---
