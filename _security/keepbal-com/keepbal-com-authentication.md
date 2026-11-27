---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keepbal-com-account-api-openapi.yml
  format: yaml
  label: KeepBal Account API
  slug: keepbal-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-account-api-openapi.yml
- filename: keepbal-com-discovery-api-openapi.yml
  format: yaml
  label: KeepBal Discovery API
  slug: keepbal-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-discovery-api-openapi.yml
- filename: keepbal-com-models-api-openapi.yml
  format: yaml
  label: KeepBal Models API
  slug: keepbal-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-models-api-openapi.yml
- filename: keepbal-com-operations-api-openapi.yml
  format: yaml
  label: KeepBal Operations API
  slug: keepbal-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-operations-api-openapi.yml
- filename: keepbal-com-pay-per-request-api-openapi.yml
  format: yaml
  label: KeepBal Pay Per Request API
  slug: keepbal-com-pay-per-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-pay-per-request-api-openapi.yml
- filename: keepbal-com-tools-api-openapi.yml
  format: yaml
  label: KeepBal Tools API
  slug: keepbal-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: KeepBal Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeepBal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: KeepBal
provider_slug: keepbal-com
scheme_count: 2
schemes:
- description: 'Send Authorization: Bearer YOUR_KEEPBAL_KEY'
  scheme: bearer
  type: http
- description: Alternative header for API key
  in: header
  name: x-api-key
  type: apiKey
slug: keepbal-com-authentication
source_filename: keepbal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: searched\nsource: https://keepbal.com/docs/authentication.md\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Send Authorization: Bearer YOUR_KEEPBAL_KEY\"\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: \"Alternative header for API key\"\n"
source_yaml_url: https://artifacts.apis.io/keepbal-com/authentication/keepbal-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API Gateway
- Tool Integration
- Prepaid Wallet
- Developer Platform
---
