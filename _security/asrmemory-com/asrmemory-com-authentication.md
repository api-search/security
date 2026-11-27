---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ASR Memory Authentication
name_suffix: Authentication
oauth_flows: []
overview: ASR Memory declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ASR Memory
provider_slug: asrmemory-com
scheme_count: 2
schemes:
- description: OAuth 2.1 with dynamic client registration (sign‑in flow)
  flows:
    authorizationCode: {}
  type: oauth2
- description: API key for tools that cannot open a sign‑in screen
  in: header
  name: X-API-Key
  type: apiKey
slug: asrmemory-com-authentication
source_filename: asrmemory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://asrmemory.com/en/docs.html\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 with dynamic client registration (sign‑in flow)\n    flows:\n      authorizationCode: {}\n  - type: apiKey\n    description: API key for tools that cannot open a sign‑in screen\n    name: X-API-Key\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/asrmemory-com/authentication/asrmemory-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Memory
- MCP
- Servers
- Collaboration
---
