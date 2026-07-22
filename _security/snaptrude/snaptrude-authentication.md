---
api_key_in: []
auth_types:
- session
description: ''
kind: authentication
layout: security
method: searched
name: Snaptrude Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snaptrude secures its APIs with session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snaptrude
provider_slug: snaptrude
scheme_count: 2
schemes:
- backend_host: https://api.snaptrude.com
  credential_store: ~/.snaptrude/auth.json
  docs: https://docs.snaptrude.com/plugin-api/plugin-development.html
  flow: '`create-snaptrude-plugin login` opens the Snaptrude app in the browser, completes sign-in, and saves credentials (including the environment API URL) to ~/.snaptrude/auth.json. register/update reuse that saved session; if not logged in they exit and prompt to run login first.'
  name: cli-session-login
  type: session
- flow: A plugin's Web Worker calls the host through the snaptrude.* API. Calls are permission-gated by the host (METHOD_NOT_PERMITTED is returned when a plugin is not allowed to call a method).
  name: plugin-runtime
  type: host-permission
slug: snaptrude-authentication
source_filename: snaptrude-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.snaptrude.com/plugin-api/plugin-development.html\nsummary:\n  types: [session]\n  model: browser-login-session\n  notes: >-\n    Snaptrude's developer surface is the client-side Plugin API. There is no\n    public API-key or OAuth surface documented. Plugin developers authenticate\n    the CLI with a browser sign-in session; the plugin runtime itself runs inside\n    the authenticated Snaptrude app session and calls the host via the\n    @snaptrude/plugin-client `snaptrude.*` RPC API.\nschemes:\n  - name: cli-session-login\n    type: session\n    flow: >-\n      `create-snaptrude-plugin login` opens the Snaptrude app in the browser,\n      completes sign-in, and saves credentials (including the environment API URL)\n      to ~/.snaptrude/auth.json. register/update reuse that saved session; if not\n      logged in they exit and prompt to run login first.\n    credential_store: ~/.snaptrude/auth.json\n    backend_host:\
  \ https://api.snaptrude.com\n    docs: https://docs.snaptrude.com/plugin-api/plugin-development.html\n  - name: plugin-runtime\n    type: host-permission\n    flow: >-\n      A plugin's Web Worker calls the host through the snaptrude.* API. Calls are\n      permission-gated by the host (METHOD_NOT_PERMITTED is returned when a plugin\n      is not allowed to call a method).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snaptrude/refs/heads/main/authentication/snaptrude-authentication.yml
summary_line: session · 2 schemes
tags:
- Company
- Design
- Architecture
- BIM
- 3D Modeling
- AEC
- Plugins
- Developer Tools
- SaaS
---
