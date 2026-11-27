---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spoken-md-transcripts-api-openapi.yml
  format: yaml
  label: Podcast Transcripts API
  slug: podcast-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-transcripts-api-openapi.yml
- filename: spoken-md-well-known-openapi.json
  format: json
  label: Podcast Transcripts API .well-known API
  slug: podcast-transcripts-api-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/_original/spoken-md-well-known-openapi.json
auth_types: []
description: Spoken API uses an opaque API key (pt_…) that can be sent as a custom header, a Bearer token, or HTTP Basic username. An OAuth token can be used only for the /mcp endpoint.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: spoken-md Authentication
name_suffix: Authentication
oauth_flows: []
overview: spoken-md declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: spoken-md
provider_slug: spoken-md
scheme_count: 1
schemes:
- evidence: Authorization code with PKCE (S256), resource=https://spoken.md/mcp
  flows:
  - authorization_code
  how_to_obtain: Register a public client via POST https://spoken.md/oauth/register, then perform the Authorization Code with PKCE flow to obtain an access token for the /mcp endpoint.
  name: Spoken MCP OAuth
  scopes:
  - mcp
  type: oauth2
slug: spoken-md-authentication
source_filename: spoken-md-authentication.yml
source_heading: Authentication Profile
source_url: https://spoken.md/auth.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://spoken.md/auth.md\nsources:\n- https://spoken.md/auth.md\ndescription: Spoken API uses an opaque API key (pt_…) that can be sent as a custom header, a Bearer token, or HTTP Basic username. An OAuth token\n  can be used only for the /mcp endpoint.\nschemes:\n- type: oauth2\n  name: Spoken MCP OAuth\n  evidence: Authorization code with PKCE (S256), resource=https://spoken.md/mcp\n  flows:\n  - authorization_code\n  scopes:\n  - mcp\n  how_to_obtain: Register a public client via POST https://spoken.md/oauth/register, then perform the Authorization Code with PKCE flow to obtain\n    an access token for the /mcp endpoint.\ndocs: https://spoken.md/auth.md\nnote: 3 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/spoken-md/authentication/spoken-md-authentication.yml
summary_line: 1 scheme
tags:
- Podcasts
- Transcripts
- Markdown
- Artificial Intelligence
---
