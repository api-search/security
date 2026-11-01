---
anonymous_access: false
api_key_in: []
api_specs:
- filename: immoapi-app-openapi-generated.yml
  format: yaml
  label: immoapi-app API
  slug: immoapi-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immoapi-app/openapi/_ae-authored/immoapi-app-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Immoapi App Authentication
name_suffix: Authentication
oauth_flows: []
overview: immoapi-app declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: immoapi-app
provider_slug: immoapi-app
scheme_count: 2
schemes:
- description: Bearer YOUR_API_KEY
  in: header
  name: Authorization
  type: apiKey
- description: Your API key
  in: header
  name: x-api-key
  type: apiKey
slug: immoapi-app-authentication
source_filename: immoapi-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://immoapi.app/documentation\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer YOUR_API_KEY\"\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"Your API key\"\n"
source_yaml_url: https://artifacts.apis.io/immoapi-app/authentication/immoapi-app-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- France
- Data
- API
- Open Data
- Property
---
