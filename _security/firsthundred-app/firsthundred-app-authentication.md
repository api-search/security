---
anonymous_access: false
api_key_in: []
auth_types: []
description: First100 authenticates clients using an API key supplied as a Bearer token in the Authorization header, or via browser sign‑in (no key).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: First100 Authentication
name_suffix: Authentication
oauth_flows: []
overview: First100 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: First100
provider_slug: firsthundred-app
scheme_count: 1
schemes:
- evidence: 'Run this in your terminal, with your own key: claude mcp add --transport http first100 https://firsthundred.app/api/mcp \ --header "Authorization: Bearer f100_your_key"'
  header: Authorization
  how_to_obtain: Generate an API key in the First100 dashboard (open API key, generate a key, and copy it while it is shown).
  location: header
  name: First100 API Key
  type: apiKey
slug: firsthundred-app-authentication
source_filename: firsthundred-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.firsthundred.app/docs/quickstart
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.firsthundred.app/docs/quickstart\nsources:\n- https://www.firsthundred.app/docs/quickstart\n- https://www.firsthundred.app/blog/claude-code-marketing\n- https://www.firsthundred.app/docs/clients\ndescription: First100 authenticates clients using an API key supplied as a Bearer token in the Authorization header, or via browser sign‑in (no\n  key).\nschemes:\n- type: apiKey\n  name: First100 API Key\n  evidence: 'Run this in your terminal, with your own key: claude mcp add --transport http first100 https://firsthundred.app/api/mcp \\ --header\n    \"Authorization: Bearer f100_your_key\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the First100 dashboard (open API key, generate a key, and copy it while it is shown).\nnote: Browser sign‑in is supported for agents like ChatGPT and Claude, which does not require an explicit API key.\n\
  docs: https://www.firsthundred.app/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/firsthundred-app/authentication/firsthundred-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MCP
- Artificial Intelligence
- Marketing
- Social
- Automation
---
