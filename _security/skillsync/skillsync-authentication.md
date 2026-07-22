---
api_key_in: []
auth_types:
- oauth2-browser
description: Skillsync has no public REST API or OpenAPI; authentication is documented for the CLI and MCP server. `skl login` opens a browser sign-in flow on skillsync.com and returns control to the CLI once the local callback completes, persisting credentials on the machine. Local-only operations (reading sessions on disk) need no login; any operation that reaches skillsync.com (upload, search published threads, skills) is login-gated. The MCP server calls the auth_status tool before any login-gated tool.
kind: authentication
layout: security
method: searched
name: Skillsync Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Skillsync secures its APIs with oauth2-browser across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Skillsync
provider_slug: skillsync
scheme_count: 1
schemes:
- description: '`skl login` opens the Skillsync sign-in flow in the browser; a local callback completes authentication and the CLI stores credentials on the machine. Confirm with `skl whoami` (CLI) or the auth_status MCP tool.'
  flow: authorizationCode
  name: browser-signin
  sources:
  - https://skillsync.com/docs/cli-reference
  - https://skillsync.com/docs/mcp-server
  type: oauth2
slug: skillsync-authentication
source_filename: skillsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://skillsync.com/docs/quickstart\ndescription: >-\n  Skillsync has no public REST API or OpenAPI; authentication is documented for\n  the CLI and MCP server. `skl login` opens a browser sign-in flow on\n  skillsync.com and returns control to the CLI once the local callback completes,\n  persisting credentials on the machine. Local-only operations (reading sessions\n  on disk) need no login; any operation that reaches skillsync.com (upload,\n  search published threads, skills) is login-gated. The MCP server calls the\n  auth_status tool before any login-gated tool.\nsummary:\n  types: [oauth2-browser]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]   # browser sign-in with local callback\nschemes:\n  - name: browser-signin\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      `skl login` opens the Skillsync sign-in flow in the browser; a local\n      callback completes authentication and the\
  \ CLI stores credentials on the\n      machine. Confirm with `skl whoami` (CLI) or the auth_status MCP tool.\n    sources: [https://skillsync.com/docs/cli-reference, https://skillsync.com/docs/mcp-server]\ngating:\n  local_only_no_auth: [list_sessions, search_sessions, get_session]\n  login_required: [upload_session, search_replay, get_replay_thread, list_workspaces, list_skills, install_skill, upload_skill]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skillsync/refs/heads/main/authentication/skillsync-authentication.yml
summary_line: oauth2-browser · 1 scheme
tags:
- Company
- Developer Tools
- AI
- Agents
- Coding Assistants
- Model Context Protocol
- CLI
- Knowledge Management
- Y Combinator
---
