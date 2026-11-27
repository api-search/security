---
anonymous_access: false
api_key_in: []
auth_types: []
description: Narrivela MCP uses OAuth2 with PKCE for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Narrivela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Narrivela declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Narrivela
provider_slug: narrivela-com
scheme_count: 1
schemes:
- evidence: The client should complete OAuth with PKCE and keep its registration and tokens for later sessions.
  flows:
  - authorization_code
  how_to_obtain: Complete browser sign‑in with your Narrivela account; the client registers automatically and uses PKCE.
  name: OAuth2
  type: oauth2
slug: narrivela-com-authentication
source_filename: narrivela-com-authentication.yml
source_heading: Authentication Profile
source_url: https://narrivela.com/integrations/mcp/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://narrivela.com/integrations/mcp/\nsources:\n- https://narrivela.com/integrations/mcp/\ndescription: Narrivela MCP uses OAuth2 with PKCE for authentication.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: The client should complete OAuth with PKCE and keep its registration and tokens for later sessions.\n  flows:\n  - authorization_code\n  how_to_obtain: Complete browser sign‑in with your Narrivela account; the client registers automatically and uses PKCE.\ndocs: https://narrivela.com/integrations/mcp/\n"
source_yaml_url: https://artifacts.apis.io/narrivela-com/authentication/narrivela-com-authentication.yml
summary_line: 1 scheme
tags:
- Voiceover
- Artificial Intelligence
- Speech
- MCP
- Audio
---
