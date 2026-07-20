---
api_key_in:
- header
auth_types:
- apiToken
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cycode Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- browser
overview: Cycode secures its APIs with apiToken and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and browser flow(s).
provider_name: Cycode
provider_slug: cycode
scheme_count: 2
schemes:
- description: A Client ID + Client Secret (personal access token) is exchanged for a short-lived JWT at POST /api/v1/auth/api-token; the JWT is sent as a Bearer token on subsequent Cycode REST API requests.
  in: header
  name: apiToken
  scheme: bearer
  sources:
  - docs.cycode.com
  type: apiKey
- description: The cycode CLI authenticates with a browser OAuth login (`cycode auth`) or with CYCODE_CLIENT_ID / CYCODE_CLIENT_SECRET client credentials.
  flow: clientCredentials
  name: oauth2-cli
  sources:
  - github.com/cycodehq/cycode-cli
  type: oauth2
slug: cycode-authentication
source_filename: cycode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cycode.com/\ndocs: https://docs.cycode.com/\nsummary:\n  types: [apiToken, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, browser]\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    scheme: bearer\n    description: >-\n      A Client ID + Client Secret (personal access token) is exchanged for a\n      short-lived JWT at POST /api/v1/auth/api-token; the JWT is sent as a\n      Bearer token on subsequent Cycode REST API requests.\n    sources: [docs.cycode.com]\n  - name: oauth2-cli\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      The cycode CLI authenticates with a browser OAuth login (`cycode auth`)\n      or with CYCODE_CLIENT_ID / CYCODE_CLIENT_SECRET client credentials.\n    sources: [github.com/cycodehq/cycode-cli]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycode/refs/heads/main/authentication/cycode-authentication.yml
summary_line: apiToken/oauth2 · 2 schemes
tags:
- Company
- Cybersecurity
- Application Security
- Software Supply Chain Security
- ASPM
- DevSecOps
- Secrets Scanning
- SAST
- SCA
- Developer Tools
- MCP
- CLI
---
