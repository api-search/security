---
anonymous_access: false
api_key_in: []
api_specs:
- filename: weatherai-io-openapi.json
  format: json
  label: Decision API
  slug: decision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weatherai-io/openapi/weatherai-io-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Weatherai Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: weatherAI.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: weatherAI.io
provider_slug: weatherai-io
scheme_count: 2
schemes:
- description: Send your key in the X-API-Key header. Authorization Bearer also works.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: 'Authorization: Bearer wai_… also accepted.'
  scheme: bearer
  type: http
slug: weatherai-io-authentication
source_filename: weatherai-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://www.weatherai.io/docs#authentication\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"Send your key in the X-API-Key header. Authorization Bearer also works.\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Authorization: Bearer wai_… also accepted.\"\n"
source_yaml_url: https://artifacts.apis.io/weatherai-io/authentication/weatherai-io-authentication.yml
summary_line: 2 schemes
tags:
- Weather
- Artificial Intelligence
- Decisions
- Forecast
---
