---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: convert.express Authentication
name_suffix: Authentication
oauth_flows: []
overview: convert.express declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: convert.express
provider_slug: convert-express
scheme_count: 3
schemes:
- description: No account or API key needed. The first job returns a robot_key; the agent passes it on every later call and it is how the server knows the jobs are the agent's. Not issued up front.
  name: robot_key
  surface: https://convert.express/mcp
  type: apiKey
- description: Signed-in variant. The client discovers sign-in through standard MCP authorization (401 with WWW-Authenticate, protected-resource metadata at /.well-known/oauth-protected-resource/mcp/account). Jobs go into the user's account; the user can disconnect the assistant, after which tools answer assistant_disconnected.
  name: MCP OAuth
  surface: https://convert.express/mcp/account
  type: oauth2
- description: Plain-text GET https://convert.express/transcript?url=<link> for assistants without MCP; same free use, preview and payment link as the MCP tools.
  name: none
  surface: https://convert.express/transcript
  type: none
slug: convert-express-authentication
source_filename: convert-express-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convert.express/llms.txt\ndocs: https://convert.express/agents\nschemes:\n- name: robot_key\n  type: apiKey\n  surface: https://convert.express/mcp\n  description: No account or API key needed. The first job returns a robot_key; the agent passes it on every later call and it is how the server knows the jobs are the agent's. Not issued up front.\n- name: MCP OAuth\n  type: oauth2\n  surface: https://convert.express/mcp/account\n  description: Signed-in variant. The client discovers sign-in through standard MCP authorization (401 with WWW-Authenticate, protected-resource metadata at /.well-known/oauth-protected-resource/mcp/account). Jobs go into the user's account; the user can disconnect the assistant, after which tools answer assistant_disconnected.\n- name: none\n  type: none\n  surface: https://convert.express/transcript\n  description: Plain-text GET https://convert.express/transcript?url=<link> for assistants without\
  \ MCP; same free use, preview and payment link as the MCP tools.\n"
source_yaml_url: https://artifacts.apis.io/convert-express/authentication/convert-express-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Transcription
- Speech-to-Text
- Audio
- Video
- Subtitles
- Artificial Intelligence
- MCP
---
