---
api_key_in:
- header
auth_types:
- apiKey
description: TestSprite authenticates with a per-account API key created in the Web Portal (Settings -> API Keys -> Create new key). The key is verified by calling GET /me before it is stored. The CLI persists it locally at ~/.testsprite/credentials (INI-style, mode 0600) and supports named profiles; the MCP server takes the key via the API_KEY environment variable. Keys carry a fixed set of scopes (see scopes/testsprite-scopes.yml).
kind: authentication
layout: security
method: searched
name: Testsprite Authentication
name_suffix: Authentication
oauth_flows: []
overview: TestSprite secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TestSprite
provider_slug: testsprite
scheme_count: 1
schemes:
- description: TestSprite API key (observed prefix `sk-`). Created once in the dashboard and shown only at creation time. Used by the CLI (`testsprite setup`), the MCP server (API_KEY env var), and Web Portal external tooling.
  docs: https://docs.testsprite.com/cli/core/authentication
  in: header
  key_prefix: sk-
  name: apiKey
  scopes_detail: scopes/testsprite-scopes.yml
  type: apiKey
  verification: GET /me
slug: testsprite-authentication
source_filename: testsprite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.testsprite.com/cli/core/authentication,\n  https://docs.testsprite.com/web-portal/admin/api-keys — TestSprite has no\n  public OpenAPI, so this profile is captured from the authentication docs\n  rather than derived from a spec.\ndescription: >-\n  TestSprite authenticates with a per-account API key created in the Web Portal\n  (Settings -> API Keys -> Create new key). The key is verified by calling\n  GET /me before it is stored. The CLI persists it locally at\n  ~/.testsprite/credentials (INI-style, mode 0600) and supports named profiles;\n  the MCP server takes the key via the API_KEY environment variable. Keys carry\n  a fixed set of scopes (see scopes/testsprite-scopes.yml).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_source: https://www.testsprite.com/dashboard/settings/apikey\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    key_prefix: sk-\n\
  \    verification: GET /me\n    description: >-\n      TestSprite API key (observed prefix `sk-`). Created once in the dashboard\n      and shown only at creation time. Used by the CLI (`testsprite setup`), the\n      MCP server (API_KEY env var), and Web Portal external tooling.\n    scopes_detail: scopes/testsprite-scopes.yml\n    docs: https://docs.testsprite.com/cli/core/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testsprite/refs/heads/main/authentication/testsprite-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Software Testing
- API Testing
- Test Automation
- AI
- Developer Tools
- Model Context Protocol
- Quality Assurance
- CI/CD
- Agentic
---
