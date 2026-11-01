---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Grundfast API
  slug: grundfast-api
  spec_type: OpenAPI
  url: https://grundfast.dk/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Grundfast Dk Authentication
name_suffix: Authentication
oauth_flows: []
overview: grundfast-dk declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: grundfast-dk
provider_slug: grundfast-dk
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: API key provided as Bearer token in Authorization header.
  scheme: bearer
  type: http
- description: API key as query parameter when header cannot be set.
  in: query
  name: token
  type: apiKey
- description: Not applicable; API uses simple API keys.
  type: oauth2
slug: grundfast-dk-authentication
source_filename: grundfast-dk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://grundfast.dk/docs/godkendelse\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key provided as Bearer token in Authorization header.\n  - type: apiKey\n    in: query\n    name: token\n    description: API key as query parameter when header cannot be set.\n  - type: oauth2\n    description: Not applicable; API uses simple API keys.\n"
source_yaml_url: https://artifacts.apis.io/grundfast-dk/authentication/grundfast-dk-authentication.yml
summary_line: 3 schemes
tags:
- RealEstate
- Geodata
- API
- Denmark
- Compatibility
---
