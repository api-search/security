---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jobo-world-openapi-generated.yml
  format: yaml
  label: jobo-world API
  slug: jobo-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobo-world/openapi/_ae-authored/jobo-world-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jobo World Authentication
name_suffix: Authentication
oauth_flows: []
overview: jobo-world declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: jobo-world
provider_slug: jobo-world
scheme_count: 1
schemes:
- description: API key required for all endpoints except GET /api/companies/{id} which is anonymous.
  in: header
  name: X-Api-Key
  type: apiKey
slug: jobo-world-authentication
source_filename: jobo-world-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://jobo.world/docs/api-reference/overview.md\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: API key required for all endpoints except GET /api/companies/{id} which is anonymous.\n"
source_yaml_url: https://artifacts.apis.io/jobo-world/authentication/jobo-world-authentication.yml
summary_line: 1 scheme
tags:
- Job Data
- API
- Recruitment
- Platform
- Data Infrastructure
---
