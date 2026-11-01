---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mnemoverse-com-memory-api-openapi.yml
  format: yaml
  label: mnemoverse-com Memory API
  slug: mnemoverse-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-memory-api-openapi.yml
auth_types: []
description: Authentication methods for Mnemoverse MCP services
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mnemoverse Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: mnemoverse-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: mnemoverse-com
provider_slug: mnemoverse-com
scheme_count: 2
schemes:
- evidence: The remote MCP server is a hosted endpoint that gives any MCP client persistent Mnemoverse memory after a one-click OAuth sign-in — no API key to copy or paste.
  how_to_obtain: User signs in via a browser consent screen; the token is stored by the client.
  name: One‑click OAuth sign‑in
  type: oauth2
- evidence: API key ( mk_live_… ) in the config
  header: Authorization
  how_to_obtain: Generate an API key in the Mnemoverse console and include it as a Bearer token in the Authorization header.
  name: API key bearer token
  type: http-bearer
slug: mnemoverse-com-authentication
source_filename: mnemoverse-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mnemoverse.com/docs/library/how-ai-agents-trust-each-other
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mnemoverse.com/docs/library/how-ai-agents-trust-each-other\nsources:\n- https://mnemoverse.com/docs/library/how-ai-agents-trust-each-other\n- https://mnemoverse.com/docs/library/memory-poisoning-secret-leak\n- https://mnemoverse.com/docs/api/remote-mcp-server\n- https://mnemoverse.com/docs/library/what-is-an-mcp-memory-server\ndescription: Authentication methods for Mnemoverse MCP services\nschemes:\n- type: oauth2\n  name: One‑click OAuth sign‑in\n  evidence: The remote MCP server is a hosted endpoint that gives any MCP client persistent Mnemoverse memory after a one-click OAuth sign-in\n    — no API key to copy or paste.\n  how_to_obtain: User signs in via a browser consent screen; the token is stored by the client.\n- type: http-bearer\n  name: API key bearer token\n  evidence: API key ( mk_live_… ) in the config\n  header: Authorization\n  how_to_obtain: Generate an\
  \ API key in the Mnemoverse console and include it as a Bearer token in the Authorization header.\ndocs: https://mnemoverse.com/docs/library/how-ai-agents-trust-each-other\n"
source_yaml_url: https://artifacts.apis.io/mnemoverse-com/authentication/mnemoverse-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Memory
- API
- Persistent
---
