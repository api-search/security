---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CaptionPipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaptionPipe declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CaptionPipe
provider_slug: captionpipe-com
scheme_count: 2
schemes:
- applies_to:
  - REST https://api.captionpipe.com/v1
  - MCP https://api.captionpipe.com/mcp
  description: 'Create a key in the dashboard under Connect. It is shown once. Sent as `Authorization: Bearer $CAPTIONPIPE_API_KEY`.'
  header: Authorization
  in: header
  name: apiKeyBearer
  scheme: bearer
  type: http
- applies_to:
  - MCP https://api.captionpipe.com/mcp
  description: Interactive clients sign in through the browser. The docs give no flow, scope or endpoint detail; the MCP protected-resource document is recorded elsewhere in this repo.
  name: oauthSignIn
  type: oauth2
slug: captionpipe-com-authentication
source_filename: captionpipe-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://captionpipe.com/docs\ndocs: https://captionpipe.com/docs\nsummary: >-\n  Interactive MCP clients sign in through the browser (OAuth); automation tools and REST use an API key\n  created in the dashboard and sent as an Authorization Bearer header. Both reach the same tools. No\n  OpenAPI is published, so this profile is read from the docs page.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: \"Create a key in the dashboard under Connect. It is shown once. Sent as `Authorization: Bearer $CAPTIONPIPE_API_KEY`.\"\n  applies_to: [REST https://api.captionpipe.com/v1, MCP https://api.captionpipe.com/mcp]\n- name: oauthSignIn\n  type: oauth2\n  description: \"Interactive clients sign in through the browser. The docs give no flow, scope or endpoint detail; the MCP protected-resource document is recorded elsewhere in this repo.\"\n  applies_to: [MCP https://api.captionpipe.com/mcp]\n\
  failure:\n  code: unauthenticated\n  http_status: 401\n  text: \"Missing or invalid key or token. HTTP 401.\"\n"
source_yaml_url: https://artifacts.apis.io/captionpipe-com/authentication/captionpipe-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Captions
- Subtitles
- Transcription
- MCP
- Automation
- AI Agents
---
