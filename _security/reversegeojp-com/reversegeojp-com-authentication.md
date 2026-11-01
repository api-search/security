---
anonymous_access: false
api_key_in: []
api_specs:
- filename: reversegeojp-com-openapi-generated.yml
  format: yaml
  label: reversegeojp-com API
  slug: reversegeojp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reversegeojp-com/openapi/_ae-authored/reversegeojp-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Reversegeojp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: reversegeojp-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: reversegeojp-com
provider_slug: reversegeojp-com
scheme_count: 2
schemes:
- description: API key passed via X-API-Key header
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token passed in Authorization header
  scheme: bearer
  type: http
slug: reversegeojp-com-authentication
source_filename: reversegeojp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://api.reversegeojp.com/\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key passed via X-API-Key header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token passed in Authorization header\n"
source_yaml_url: https://artifacts.apis.io/reversegeojp-com/authentication/reversegeojp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Geocoding
- Japan
- API
- Location
---
