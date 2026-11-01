---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nobil Authentication
name_suffix: Authentication
oauth_flows: []
overview: NOBIL (Enova) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NOBIL (Enova)
provider_slug: nobil
scheme_count: 1
schemes:
- description: API key provided after registration; required for all requests.
  in: header
  name: x-api-key
  type: apiKey
slug: nobil-authentication
source_filename: nobil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://info.nobil.no/images/API_NOBIL_Documentation_v3_20260816.pdf\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key provided after registration; required for all requests."
source_yaml_url: https://artifacts.apis.io/nobil/authentication/nobil-authentication.yml
summary_line: 1 scheme
tags:
- EV
- Charging
- Energy
- Data
- Norway
- Transportation
---
