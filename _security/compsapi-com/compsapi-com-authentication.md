---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compsapi-com-comps-api-openapi.yml
  format: yaml
  label: compsapi-com Comps API
  slug: compsapi-com-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-comps-api-openapi.yml
- filename: compsapi-com-health-api-openapi.yml
  format: yaml
  label: compsapi-com Health API
  slug: compsapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-health-api-openapi.yml
- filename: compsapi-com-sold-api-openapi.yml
  format: yaml
  label: compsapi-com Sold API
  slug: compsapi-com-sold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-sold-api-openapi.yml
- filename: compsapi-com-usage-api-openapi.yml
  format: yaml
  label: compsapi-com Usage API
  slug: compsapi-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Compsapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: compsapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: compsapi-com
provider_slug: compsapi-com
scheme_count: 2
schemes:
- description: API key passed in header
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token alternative
  scheme: bearer
  type: http
slug: compsapi-com-authentication
source_filename: compsapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://compsapi.com/docs\nschemes:\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: API key passed in header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token alternative"
source_yaml_url: https://artifacts.apis.io/compsapi-com/authentication/compsapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- eBay
- Data
- Pricing
- Marketplace
---
