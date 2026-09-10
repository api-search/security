---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bettip-draws-api-openapi.json
  format: json
  label: BetTip Draws API
  slug: bettip-draws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bettip-draws-api/refs/heads/main/openapi/bettip-draws-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Bettip Draws Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetTip Draws API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: BetTip Draws API
provider_slug: bettip-draws-api
scheme_count: 0
schemes: []
slug: bettip-draws-api-authentication
source_filename: bettip-draws-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://bettip.co.za/api/ + openapi/bettip-draws-api-openapi.json\ndocs: https://bettip.co.za/api/\nnote: >-\n  Deliberately unauthenticated: the docs state \"No key, no account, open to\n  any origin\" and the OpenAPI declares no securitySchemes. Verified live —\n  GET https://bettip.co.za/api/v1/uk49s/latest.json returns 200 with\n  Access-Control-Allow-Origin: * and no credentials. Attribution to BetTip\n  (link to https://bettip.co.za/) is the only usage condition.\nschemes: []\nauthentication:\n  required: false\n  type: none\n  cors: open\n  conditions:\n    - Attribution to BetTip with a link to https://bettip.co.za/ wherever the data is shown\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettip-draws-api/refs/heads/main/authentication/bettip-draws-api-authentication.yml
summary_line: 0 schemes
tags:
- Lottery results
- UK49s
- Gosloto
- SA National Lottery
- JSON
- CSV
- OpenAPI
- Sports/Betting data
- Reference data
- Open data
- Gambling & Betting
---
