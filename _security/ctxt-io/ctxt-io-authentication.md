---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Context Authentication
name_suffix: Authentication
oauth_flows: []
overview: Context declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Context
provider_slug: ctxt-io
scheme_count: 3
schemes:
- description: The MCP server is stateless Streamable HTTP with "no session ids, no authentication" and "No account, no API key, nothing to install."
  name: anonymous
  type: none
- description: create_context returns "a delete_token that authorizes later deletion — treat the token as a secret." It is per-link, not an account credential.
  in: tool argument (delete_context)
  name: delete_token
  type: bearer-token
- description: Pro links (ttl=30d) may set a password; read_context takes "password for protected links". "Password protection is an access gate, not encryption."
  in: tool argument (read_context / create_context)
  name: link password
  type: password
slug: ctxt-io-authentication
source_filename: ctxt-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://ctxt.io/mcp/docs\ndocs: https://ctxt.io/mcp/docs\nschemes:\n- type: none\n  name: anonymous\n  description: 'The MCP server is stateless Streamable HTTP with \"no session ids, no authentication\" and \"No account, no API key, nothing to install.\"'\n- type: bearer-token\n  name: delete_token\n  in: tool argument (delete_context)\n  description: 'create_context returns \"a delete_token that authorizes later deletion — treat the token as a secret.\" It is per-link, not an account credential.'\n- type: password\n  name: link password\n  in: tool argument (read_context / create_context)\n  description: 'Pro links (ttl=30d) may set a password; read_context takes \"password for protected links\". \"Password protection is an access gate, not encryption.\"'\nnote: Links themselves are bearer-accessible (\"anyone who has the URL can read it until it expires\"). No OAuth, so no scopes artifact.\n"
source_yaml_url: https://artifacts.apis.io/ctxt-io/authentication/ctxt-io-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Pastebin
- Content Sharing
- MCP
- AI Agents
- Browser Extension
- Developer Tools
---
