---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tinkermode-com-openapi-generated.yml
  format: yaml
  label: Mode API
  slug: tinkermode-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinkermode-com/openapi/_ae-authored/tinkermode-com-openapi-generated.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tinkermode Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mode
provider_slug: tinkermode-com
scheme_count: 1
schemes:
- description: 'Authorization header for MODE API calls. Example: Authorization: ModeCloud abc123'
  format: ModeCloud <AUTH_CODE>
  in: header
  name: ModeCloudAuth
  parameter: Authorization
  prefix: ModeCloud
  purpose: Identify the client to the MODE API. The token is a bearer token issued via the console.
  scoped: false
  sources:
  - https://dev.tinkermode.com/mode-api/02-making-requests
  type: apiKey
slug: tinkermode-com-authentication
source_filename: tinkermode-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://dev.tinkermode.com/mode-api/02-making-requests\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  note: >-\n    Authentication uses the Authorization header with the format \"ModeCloud <AUTH_CODE>\".\n    No OAuth flows are documented.\nschemes:\n  - name: ModeCloudAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: ModeCloud <AUTH_CODE>\n    prefix: ModeCloud \n    purpose: >-\n      Identify the client to the MODE API. The token is a bearer token issued via the console.\n    description: \"Authorization header for MODE API calls. Example: Authorization: ModeCloud abc123\"\n    scoped: false\n    sources:\n      - https://dev.tinkermode.com/mode-api/02-making-requests\n"
source_yaml_url: https://artifacts.apis.io/tinkermode-com/authentication/tinkermode-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Data-Platform
- Industrial
- Construction
- Operations
- Company
---
