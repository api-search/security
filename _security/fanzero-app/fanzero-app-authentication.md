---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FanZero Authentication
name_suffix: Authentication
oauth_flows: []
overview: FanZero declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FanZero
provider_slug: fanzero-app
scheme_count: 1
schemes:
- evidence: 'claude mcp add --transport http fanzero https://fanzero.app/mcp --header "Authorization: Bearer $FANZERO_API_KEY"'
  header: Authorization
  how_to_obtain: Set the environment variable FANZERO_API_KEY and use it as a Bearer token in the Authorization header.
  location: header
  name: Authorization
  type: apiKey
slug: fanzero-app-authentication
source_filename: fanzero-app-authentication.yml
source_heading: Authentication Profile
source_url: https://fanzero.app/docs/publish-with-claude-code
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fanzero.app/docs/publish-with-claude-code\nsources:\n- https://fanzero.app/docs/publish-with-claude-code\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'claude mcp add --transport http fanzero https://fanzero.app/mcp --header \"Authorization: Bearer $FANZERO_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Set the environment variable FANZERO_API_KEY and use it as a Bearer token in the Authorization header.\ndocs: https://fanzero.app/docs/publish-with-claude-code\n"
source_yaml_url: https://artifacts.apis.io/fanzero-app/authentication/fanzero-app-authentication.yml
summary_line: 1 scheme
tags:
- Gaming
- Influencer Marketing
- Revenue Share
- Indie Games
- Platform
---
