---
anonymous_access: false
api_key_in: []
api_specs:
- filename: valet-dev-install-api-openapi.yml
  format: yaml
  label: valet-dev Install API
  slug: valet-dev-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valet-dev/openapi/valet-dev-install-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: valet-dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: valet-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: valet-dev
provider_slug: valet-dev
scheme_count: 1
schemes:
- authorizationUrl: https://auth.valet.dev/verify
  description: OAuth device flow for Valet CLI authentication.
  flow: device_code
  tokenUrl: https://auth.valet.dev/token
  type: oauth2
slug: valet-dev-authentication
source_filename: valet-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://www.valet.dev/docs/cli\nschemes:\n  - type: oauth2\n    flow: device_code\n    authorizationUrl: https://auth.valet.dev/verify\n    tokenUrl: https://auth.valet.dev/token\n    description: OAuth device flow for Valet CLI authentication.\n"
source_yaml_url: https://artifacts.apis.io/valet-dev/authentication/valet-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Platform
- Citizen-Developer
- Automation
- Integration
---
