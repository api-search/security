---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mastheads-app-openapi-generated.yml
  format: yaml
  label: Mastheads API
  slug: mastheads-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mastheads-app/openapi/_ae-authored/mastheads-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Mastheads API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Mastheads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastheads declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Mastheads
provider_slug: mastheads-app
scheme_count: 3
schemes:
- evidence: An MCP client that signs in with OAuth - Codex, Claude, and any client that supports it - mints its own credential when you connect it, with nothing to paste and no key on disk.
  name: OAuth
  type: oauth2
- evidence: Everything else, including a script or server calling /v1 directly, authenticates with an API key sent as a bearer token.
  header: Authorization
  how_to_obtain: Mint one in the dashboard under Settings → Account → Developer.
  location: header
  name: API key (Bearer)
  type: apiKey
- evidence: 'Sending the key Send it as an Authorization: Bearer header. An X-Api-Key header works too, if that fits your tooling better.'
  header: X-Api-Key
  how_to_obtain: Mint one in the dashboard under Settings → Account → Developer.
  location: header
  name: API key (X-Api-Key)
  type: apiKey
slug: mastheads-app-authentication
source_filename: mastheads-app-authentication.yml
source_heading: Authentication Profile
source_url: https://mastheads.app/docs/api/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mastheads.app/docs/api/authentication\nsources:\n- https://mastheads.app/docs/api/authentication\n- https://mastheads.app/docs/getting-started/quick-start\n- https://mastheads.app/docs/getting-started/how-an-article-happens\n- https://mastheads.app/docs/getting-started/the-nine-desks\ndescription: Authentication methods for Mastheads API\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: An MCP client that signs in with OAuth - Codex, Claude, and any client that supports it - mints its own credential when you connect\n    it, with nothing to paste and no key on disk.\n- type: apiKey\n  name: API key (Bearer)\n  evidence: Everything else, including a script or server calling /v1 directly, authenticates with an API key sent as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Mint one in the dashboard under Settings → Account → Developer.\n\
  - type: apiKey\n  name: API key (X-Api-Key)\n  evidence: 'Sending the key Send it as an Authorization: Bearer header. An X-Api-Key header works too, if that fits your tooling better.'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Mint one in the dashboard under Settings → Account → Developer.\ndocs: https://mastheads.app/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/mastheads-app/authentication/mastheads-app-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Newsroom
- Content
- Publishing
---
