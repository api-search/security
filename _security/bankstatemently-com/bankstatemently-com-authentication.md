---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Bankstatemently API
  slug: bankstatemently-api
  spec_type: OpenAPI
  url: https://api.bankstatemently.com/v1/openapi.json
- filename: bankstatemently-com-v1-openapi.json
  format: json
  label: Bankstatemently API V1 API
  slug: bankstatemently-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankstatemently-com/openapi/_original/bankstatemently-com-v1-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bankstatemently Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bankstatemently declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bankstatemently
provider_slug: bankstatemently-com
scheme_count: 2
schemes:
- description: API key provided via X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: 'Clerk JWT token in Authorization: Bearer header for frontend integrations.'
  scheme: bearer
  type: http
slug: bankstatemently-com-authentication
source_filename: bankstatemently-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://bankstatemently.com/developers/api\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"API key provided via X-API-Key header.\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Clerk JWT token in Authorization: Bearer header for frontend integrations.\"\n"
source_yaml_url: https://artifacts.apis.io/bankstatemently-com/authentication/bankstatemently-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Banking
- Data Conversion
- Software-as-a-Service
---
