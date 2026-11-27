---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clip Studio AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clip Studio AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clip Studio AI
provider_slug: clipstudio-ai
scheme_count: 1
schemes:
- applies_to: https://clipstudio.ai/api/mcp
  authorization_server: https://clipstudio.ai
  dynamic_client_registration: true
  evidence:
  - One-click OAuth. MCP clients register themselves and open a browser. You approve. Tokens stay on the agent; we store hashes.
  - Connect at https://clipstudio.ai/api/mcp. Sign in once. No API key in the happy path.
  - Point the agent at https://clipstudio.ai/api/mcp. No client id. No pasted key.
  flow: authorization_code
  name: mcp-oauth
  scopes:
  - clipstudio
  type: oauth2
slug: clipstudio-ai-authentication
source_filename: clipstudio-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clipstudio.ai/mcp.md\ndocs: https://clipstudio.ai/mcp\nsummary: 'The only programmatic surface is the remote MCP server at https://clipstudio.ai/api/mcp. It uses OAuth with client self-registration and browser approval; no API keys are issued in the documented flow. Anonymous calls are refused (pre-flight probe: initialize returned 401, recorded in apis.yml as scope clipstudio, authorization server https://clipstudio.ai).'\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  dynamic_client_registration: true\n  scopes:\n  - clipstudio\n  authorization_server: https://clipstudio.ai\n  applies_to: https://clipstudio.ai/api/mcp\n  evidence:\n  - 'One-click OAuth. MCP clients register themselves and open a browser. You approve. Tokens stay on the agent; we store hashes.'\n  - 'Connect at https://clipstudio.ai/api/mcp. Sign in once. No API key in the happy path.'\n  - 'Point the agent at https://clipstudio.ai/api/mcp.\
  \ No client id. No pasted key.'\n"
source_yaml_url: https://artifacts.apis.io/clipstudio-ai/authentication/clipstudio-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Video
- Video Generation
- Generative AI
- Image Generation
- Short-Form Video
- Video Ads
- MCP
---
