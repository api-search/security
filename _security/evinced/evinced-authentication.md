---
api_key_in:
- env
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Evinced Authentication
name_suffix: Authentication
oauth_flows: []
overview: evinced secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: evinced
provider_slug: evinced
scheme_count: 1
schemes:
- credentials:
  - EVINCED_SERVICE_ID
  - EVINCED_SERVICE_ACCOUNT_ID
  - EVINCED_API_KEY
  - EVINCED_ACCESS_TOKEN
  in: env
  name: EvincedApiKey
  sources:
  - https://developer.evinced.com/mcp-servers/web-mcp-server
  - https://developer.evinced.com/mcp-servers/mobile-mcp-server
  type: apiKey
slug: evinced-authentication
source_filename: evinced-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.evinced.com/mcp-servers/web-mcp-server\ndocs: https://developer.evinced.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [env]\n  oauth2_flows: []\n  notes: >-\n    Evinced SDKs and MCP servers authenticate with a service account\n    identifier plus an API key, supplied as environment variables. An offline\n    access token is available as an alternative for the mobile server. There is\n    no public OpenAPI-declared securityScheme (Evinced ships no public REST\n    API); this profile is derived from the published SDK/MCP setup docs.\nschemes:\n  - name: EvincedApiKey\n    type: apiKey\n    in: env\n    credentials:\n      - EVINCED_SERVICE_ID           # web MCP / web SDKs\n      - EVINCED_SERVICE_ACCOUNT_ID   # mobile MCP / mobile SDKs\n      - EVINCED_API_KEY\n      - EVINCED_ACCESS_TOKEN         # offline alternative (mobile)\n    sources: [https://developer.evinced.com/mcp-servers/web-mcp-server, https://developer.evinced.com/mcp-servers/mobile-mcp-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evinced/refs/heads/main/authentication/evinced-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Accessibility
- Testing
- Quality Assurance
- Devops
- Web
- Mobile
- MCP
- SDK
- Artificial Intelligence
---
