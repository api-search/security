---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alfanestlabs-com-openapi-generated.yml
  format: yaml
  label: AlfaNest Labs API
  slug: alfanestlabs-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfanestlabs-com/openapi/_ae-authored/alfanestlabs-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Alfanestlabs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlfaNest Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AlfaNest Labs
provider_slug: alfanestlabs-com
scheme_count: 2
schemes:
- description: Project key starting with an_live_, used for machine-to-machine calls.
  in: header
  name: Authorization
  type: apiKey
- bearerFormat: JWT
  description: Session token obtained after signing in at /login, used for authenticated routes.
  scheme: bearer
  type: http
slug: alfanestlabs-com-authentication
source_filename: alfanestlabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://alfanestlabs.com/veridex/docs\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Project key starting with an_live_, used for machine-to-machine calls.\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Session token obtained after signing in at /login, used for authenticated routes.\"\n"
source_yaml_url: https://artifacts.apis.io/alfanestlabs-com/authentication/alfanestlabs-com-authentication.yml
summary_line: 2 schemes
tags:
- Data Security
- API Risk
- Machine Identity
- Artificial Intelligence
- Privacy
---
