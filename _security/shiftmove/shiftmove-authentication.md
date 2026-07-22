---
api_key_in: []
api_specs:
- filename: shiftmove-fleet-openapi.json
  format: json
  label: Avrios Fleet-API
  slug: avrios-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-fleet-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shiftmove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shiftmove secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shiftmove
provider_slug: shiftmove
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Set `Authorization: Basic {base64(username:password)}` on every request. Documented in the Fleet-API "Access and usage / Authorization" section.'
  name: basicAuth
  scheme: basic
  sources:
  - docs
  type: http
slug: shiftmove-authentication
source_filename: shiftmove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.avrios.com/\ndocs: https://developers.avrios.com/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Avrios Fleet-API (the API surface of Shiftmove GmbH) uses HTTP Basic\n    authentication. A base64-encoded `username:password` credential pair must be\n    supplied on every request via the `Authorization: Basic {credentials}` header.\n    Credentials are issued by Avrios/Shiftmove per company account. The published\n    Swagger 2.0 document does not declare a `securityDefinitions` block, so this\n    profile is captured from the API documentation prose rather than derived from\n    the spec.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. Set `Authorization: Basic {base64(username:password)}`\n      on every request. Documented in the Fleet-API \"Access and usage / Authorization\"\
  \n      section.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/authentication/shiftmove-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fleet Management
- Mobility
- Automotive
- Telematics
- Vehicles
- Fleet API
- SaaS
---
