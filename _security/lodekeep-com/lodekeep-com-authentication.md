---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as described on the Security page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lodekeep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lodekeep declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lodekeep
provider_slug: lodekeep-com
scheme_count: 2
schemes:
- evidence: command-line clients use scoped, revocable API keys.
  name: API Key
  type: apiKey
- evidence: remote connectors (Claude web, ChatGPT, Grok) use OAuth 2.1 with PKCE
  name: OAuth 2.1 with PKCE
  type: oauth2
slug: lodekeep-com-authentication
source_filename: lodekeep-com-authentication.yml
source_heading: Authentication Profile
source_url: https://lodekeep.com/security
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lodekeep.com/security\nsources:\n- https://lodekeep.com/security\ndescription: Authentication methods as described on the Security page.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: command-line clients use scoped, revocable API keys.\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: remote connectors (Claude web, ChatGPT, Grok) use OAuth 2.1 with PKCE\ndocs: https://lodekeep.com/security\n"
source_yaml_url: https://artifacts.apis.io/lodekeep-com/authentication/lodekeep-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Memory
- MCP
- Claude
- Productivity
---
