---
anonymous_access: false
api_key_in: []
api_specs:
- filename: placid-openai-api-openapi.yml
  format: yaml
  label: Placid Openai API
  slug: placid-openai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placid/openapi/placid-openai-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Placid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Placid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Placid
provider_slug: placid
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API token passed in Authorization header as Bearer token.
  header: Authorization
  scheme: bearer
  type: http
slug: placid-authentication
source_filename: placid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://placid.app/docs/2.0/rest/authentication\nname: Placid authentication\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API token passed in Authorization header as Bearer token.\n    header: Authorization\n"
source_yaml_url: https://artifacts.apis.io/placid/authentication/placid-authentication.yml
summary_line: 1 scheme
tags:
- Automation
- Creative
- API
- Image-Generation
- No-Code
---
