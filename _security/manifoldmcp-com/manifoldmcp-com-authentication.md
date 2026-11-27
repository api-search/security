---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Manifold supports two authentication methods: OAuth sign‑in and API keys. Both result in a bearer token sent to https://mcp.manifoldmcp.com/mcp.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Manifold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Manifold declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Manifold
provider_slug: manifoldmcp-com
scheme_count: 1
schemes:
- evidence: Sign in with OAuth from your client, or send an API key. Both spend one workspace's credits.
  how_to_obtain: Your client opens the Manifold sign‑in page, signs in with Google or email, and the server publishes its OAuth metadata at https://mcp.manifoldmcp.com/.well-known/oauth-protected-resource/mcp.
  name: OAuth
  type: oauth2
slug: manifoldmcp-com-authentication
source_filename: manifoldmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.manifoldmcp.com/docs/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.manifoldmcp.com/docs/authentication.md\nsources:\n- https://www.manifoldmcp.com/docs/authentication.md\n- https://www.manifoldmcp.com/docs/authentication\n- https://www.manifoldmcp.com/docs/index.md\n- https://www.manifoldmcp.com/blog/how-to-track-competitors.md\ndescription: 'Manifold supports two authentication methods: OAuth sign‑in and API keys. Both result in a bearer token sent to https://mcp.manifoldmcp.com/mcp.'\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign in with OAuth from your client, or send an API key. Both spend one workspace's credits.\n  how_to_obtain: Your client opens the Manifold sign‑in page, signs in with Google or email, and the server publishes its OAuth metadata at https://mcp.manifoldmcp.com/.well-known/oauth-protected-resource/mcp.\ndocs: https://www.manifoldmcp.com/docs/authentication.md\nnote: 1 extracted row(s) were dropped\
  \ because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/manifoldmcp-com/authentication/manifoldmcp-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketing
- Artificial Intelligence
- Data
- SEO
---
