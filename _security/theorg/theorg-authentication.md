---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Theorg Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Org secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Org
provider_slug: theorg
scheme_count: 1
schemes:
- description: 'All requests authenticate with an account-scoped API key passed in the X-Api-Key header. Keys are created from the developer subscription page after creating a free The Org account (each key is given an informative name). All requests must be made over HTTPS; plain HTTP calls fail. The same key authenticates the REST API and the MCP endpoint.

    '
  in: header
  name: X-Api-Key
  sources:
  - https://developers.theorg.com/api/get-started
  type: apiKey
slug: theorg-authentication
source_filename: theorg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.theorg.com/api/get-started\ndocs: https://developers.theorg.com/api/key-concepts\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    name: X-Api-Key\n    description: >\n      All requests authenticate with an account-scoped API key passed in the\n      X-Api-Key header. Keys are created from the developer subscription page after\n      creating a free The Org account (each key is given an informative name). All\n      requests must be made over HTTPS; plain HTTP calls fail. The same key authenticates\n      the REST API and the MCP endpoint.\n    sources: [https://developers.theorg.com/api/get-started]\ntransport: https-required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorg/refs/heads/main/authentication/theorg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Organizational Charts
- People Data
- Sales Intelligence
- Prospecting
- Org Chart
- B2B Data
- MCP
---
