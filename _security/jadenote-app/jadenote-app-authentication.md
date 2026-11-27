---
anonymous_access: false
api_key_in: []
auth_types: []
description: Jade Note authenticates API requests to Claude Code routines using an API token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jade Note Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jade Note declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jade Note
provider_slug: jadenote-app
scheme_count: 1
schemes:
- evidence: Copy the fire URL and the API token . The token is shown only once, when you save, so copy it before closing the dialog.
  header: Authorization
  how_to_obtain: The token is generated when saving the Claude Code routine and displayed once in the dialog.
  location: header
  name: API token
  type: http-bearer
slug: jadenote-app-authentication
source_filename: jadenote-app-authentication.yml
source_heading: Authentication Profile
source_url: https://jadenote.app/docs/claude-code-routines/
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jadenote.app/docs/claude-code-routines/\nsources:\n- https://jadenote.app/docs/claude-code-routines/\ndescription: Jade Note authenticates API requests to Claude Code routines using an API token.\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: Copy the fire URL and the API token . The token is shown only once, when you save, so copy it before closing the dialog.\n  location: header\n  header: Authorization\n  how_to_obtain: The token is generated when saving the Claude Code routine and displayed once in the dialog.\nnote: No other authentication schemes are documented on the page.\ndocs: https://jadenote.app/docs/claude-code-routines/\n"
source_yaml_url: https://artifacts.apis.io/jadenote-app/authentication/jadenote-app-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Note Taking
- Collaboration
- MCP
- Productivity
- Company
---
