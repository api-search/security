---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Summer Engine API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: summerengine-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: summerengine-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: summerengine-com
provider_slug: summerengine-com
scheme_count: 1
schemes:
- evidence: 'A Summer sign-in: an OAuth 2.1 access token, valid one hour. Sign in once with npx -y summer-engine login, then print a token with summer token.'
  header: Authorization
  how_to_obtain: Run `npx -y summer-engine@latest login` to sign in once, then print a token with `summer token`.
  location: header
  name: bearer
  type: http-bearer
slug: summerengine-com-authentication
source_filename: summerengine-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.summerengine.com/essentials/authentication.md
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.summerengine.com/essentials/authentication.md\nsources:\n- https://docs.summerengine.com/essentials/authentication.md\n- https://docs.summerengine.com/api/reference/get-voices-preview-token.md\n- https://docs.summerengine.com/quickstarts/fresh-project.md\n- https://docs.summerengine.com/quickstarts/coding-agent.md\ndescription: Authentication schemes for Summer Engine API\nschemes:\n- type: http-bearer\n  name: bearer\n  evidence: 'A Summer sign-in: an OAuth 2.1 access token, valid one hour. Sign in once with npx -y summer-engine login, then print a token with\n    summer token.'\n  location: header\n  header: Authorization\n  how_to_obtain: Run `npx -y summer-engine@latest login` to sign in once, then print a token with `summer token`.\ndocs: https://docs.summerengine.com/essentials/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/summerengine-com/authentication/summerengine-com-authentication.yml
summary_line: 1 scheme
tags:
- Game Engine
- AI Tools
- Asset Store
- Multiplayer
- Publishing
- Analytics
---
