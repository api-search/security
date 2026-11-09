---
anonymous_access: false
api_key_in: []
api_specs:
- filename: serpresult-com-account-api-openapi.yml
  format: yaml
  label: SerpResult Account API
  slug: serpresult-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-account-api-openapi.yml
- filename: serpresult-com-api-keys-api-openapi.yml
  format: yaml
  label: SerpResult API keys API
  slug: serpresult-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-api-keys-api-openapi.yml
- filename: serpresult-com-billing-api-openapi.yml
  format: yaml
  label: SerpResult Billing API
  slug: serpresult-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-billing-api-openapi.yml
- filename: serpresult-com-meta-api-openapi.yml
  format: yaml
  label: SerpResult Meta API
  slug: serpresult-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-meta-api-openapi.yml
- filename: serpresult-com-search-api-openapi.yml
  format: yaml
  label: SerpResult Search API
  slug: serpresult-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-search-api-openapi.yml
- filename: serpresult-com-usage-api-openapi.yml
  format: yaml
  label: SerpResult Usage API
  slug: serpresult-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Serpresult Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: SerpResult declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SerpResult
provider_slug: serpresult-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Public API calls send a secret key in the Authorization header: Authorization: Bearer <key>'
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: serpresult-com-authentication
source_filename: serpresult-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.serpresult.com/api/authentication/\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Public API calls send a secret key in the Authorization header: Authorization: Bearer <key>\"\n    name: Authorization\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/serpresult-com/authentication/serpresult-com-authentication.yml
summary_line: 1 scheme
tags:
- Search
- SERP
- Data
- JSON
- Cloud
---
