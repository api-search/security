---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Orisu MCP supports OAuth for interactive chat clients and API keys for scripts.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Orisu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orisu declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Orisu
provider_slug: orisu-ai
scheme_count: 2
schemes:
- evidence: When you add Orisu as a connector in Claude or ChatGPT, the host runs an OAuth flow against the Orisu web app.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Host dynamically registers as an OAuth client, the user signs in and approves scopes, then the host receives an authorization code and exchanges it at the token endpoint to obtain access and refresh tokens.
  location: header
  name: OAuth
  scopes:
  - agents:read
  - agents:write
  - runs:read
  - runs:execute
  - apps:read
  - apps:execute
  - assets:write
  - openid
  - offline_access
  type: http-bearer
- evidence: 'Send it as a Bearer token to the same endpoint:'
  header: Authorization
  how_to_obtain: Generate an API key from the Orisu dashboard Settings → API Keys; the key format is pk_live_*.
  location: header
  name: API Key
  type: http-bearer
slug: orisu-ai-authentication
source_filename: orisu-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.orisu.ai/mcp/authentication.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.orisu.ai/mcp/authentication.md\nsources:\n- https://docs.orisu.ai/mcp/authentication.md\n- https://docs.orisu.ai/guides/quickstart.md\n- https://docs.orisu.ai/mcp/quickstart.md\ndescription: Authentication for Orisu MCP supports OAuth for interactive chat clients and API keys for scripts.\nschemes:\n- type: http-bearer\n  name: OAuth\n  evidence: When you add Orisu as a connector in Claude or ChatGPT, the host runs an OAuth flow against the Orisu web app.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  scopes:\n  - agents:read\n  - agents:write\n  - runs:read\n  - runs:execute\n  - apps:read\n  - apps:execute\n  - assets:write\n  - openid\n  - offline_access\n  how_to_obtain: Host dynamically registers as an OAuth client, the user signs in and approves scopes, then the host receives an authorization\n    code and exchanges it at the\
  \ token endpoint to obtain access and refresh tokens.\n- type: http-bearer\n  name: API Key\n  evidence: 'Send it as a Bearer token to the same endpoint:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key from the Orisu dashboard Settings → API Keys; the key format is pk_live_*.\ndocs: https://docs.orisu.ai/mcp/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/orisu-ai/authentication/orisu-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Advertising
- Creative
- Marketing
- Video
---
