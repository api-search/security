---
anonymous_access: false
api_key_in: []
api_specs:
- filename: uptybots-com-openapi-generated.yml
  format: yaml
  label: uptybots-com API
  slug: uptybots-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptybots-com/openapi/_ae-authored/uptybots-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Uptybots Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: uptybots-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: uptybots-com
provider_slug: uptybots-com
scheme_count: 2
schemes:
- description: API key passed in X-API-Key header
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: API key passed as Bearer token in Authorization header
  scheme: bearer
  type: http
slug: uptybots-com-authentication
source_filename: uptybots-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://uptybots.com/docs/api#authentication\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key passed in X-API-Key header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key passed as Bearer token in Authorization header\n"
source_yaml_url: https://artifacts.apis.io/uptybots-com/authentication/uptybots-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Monitoring
- Uptime
- Artificial Intelligence
- MCP
---
