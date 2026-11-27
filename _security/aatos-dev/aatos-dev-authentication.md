---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AATOS Authentication
name_suffix: Authentication
oauth_flows: []
overview: AATOS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AATOS
provider_slug: aatos-dev
scheme_count: 1
schemes:
- description: API key provided after on-chain payment activation
  in: header
  name: x-api-key
  type: apiKey
slug: aatos-dev-authentication
source_filename: aatos-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://aatos.dev/api/access/pricing\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"API key provided after on-chain payment activation\"\n"
source_yaml_url: https://artifacts.apis.io/aatos-dev/authentication/aatos-dev-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Tokenization
- MCP
- Robinhood Chain
- Cryptocurrency
---
