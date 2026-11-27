---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Digital Maker AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Maker AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Digital Maker AI
provider_slug: digitalmaker-ai
scheme_count: 3
schemes:
- description: Create a key in Account Settings, under the API tab. The key is shown once and never stored in a readable form.
  header: x-dmai-key
  in: header
  key_prefix: dmai_live_
  name: dmai-key
  type: apiKey
- description: 'The agents page: "Connect over HTTP to https://digitalmaker.ai/mcp with your key as a Bearer token".'
  name: bearer
  scheme: bearer
  source: https://digitalmaker.ai/agents
  type: http
- description: Clients that speak MCP natively (n8n, Make, Cursor, ChatGPT connectors) usually take the key in the URL instead. Both reach the same server and accept the same key.
  in: path
  name: key-in-url
  type: apiKey
  url_template: https://digitalmaker.ai/mcp/YOUR_KEY
slug: digitalmaker-ai-authentication
source_filename: digitalmaker-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://digitalmaker.ai/api-docs\ndocs: https://digitalmaker.ai/api-docs\nschemes:\n- name: dmai-key\n  type: apiKey\n  in: header\n  header: x-dmai-key\n  key_prefix: dmai_live_\n  description: Create a key in Account Settings, under the API tab. The key is shown once and never stored in a readable form.\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'The agents page: \"Connect over HTTP to https://digitalmaker.ai/mcp with your key as a Bearer token\".'\n  source: https://digitalmaker.ai/agents\n- name: key-in-url\n  type: apiKey\n  in: path\n  url_template: https://digitalmaker.ai/mcp/YOUR_KEY\n  description: Clients that speak MCP natively (n8n, Make, Cursor, ChatGPT connectors) usually take the key in the URL instead. Both reach the same server and accept the same key.\nkey_lifecycle:\n  shown_once: true\n  revocation: Revoking takes effect immediately.\n  expiry: Keys that go unused for 90 days expire\
  \ on their own.\n  per_project_keys: use a separate named key per project so revoking one thing does not break everything else.\noauth: The Claude connector is built from the AI Connector tab in Account Settings; no OAuth scopes are documented.\n"
source_yaml_url: https://artifacts.apis.io/digitalmaker-ai/authentication/digitalmaker-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Video Generation
- Faceless Video
- YouTube
- Content Creation
- Digital Products
- MCP
---
