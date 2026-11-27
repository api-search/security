---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CoSchedule Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoSchedule declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CoSchedule
provider_slug: coschedule-com
scheme_count: 3
schemes:
- authorization_server: https://accounts-billing.coschedule.com
  bearer_methods:
  - header
  docs_quote: You sign in with your own CoSchedule account, and Claude sees only what that account can see.
  evidence: https://platform.coschedule.com/.well-known/oauth-protected-resource/mcp
  name: mcp-oauth
  scopes_supported:
  - openid
  surface: MCP server (https://platform.coschedule.com/mcp)
  type: oauth2
- docs: https://coschedule.com/support/integrations/other-tools/connect-other-tools-with-zapier
  docs_quote: Each calendar has its own API key. To connect several calendars, connect each one with its own key.
  name: zapier-calendar-api-key
  surface: Zapier connection
  type: apiKey
- docs: https://coschedule.com/support/integrations/other-tools/use-webhooks
  docs_quote: CoSchedule sends the token in a Verify-Token header with every call, so your endpoint can check that the call came from CoSchedule.
  header: Verify-Token
  in: header
  name: webhook-verify-token
  surface: outbound webhooks (CoSchedule to your endpoint)
  type: apiKey
slug: coschedule-com-authentication
source_filename: coschedule-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coschedule.com/support/integrations/ai-chat-apps/connect-claude-to-coschedule\ndocs: https://coschedule.com/support/integrations/ai-chat-apps/use-claude-and-chatgpt-with-coschedule\nsummary: CoSchedule has no public REST API. Its MCP server uses OAuth sign-in with the user's own CoSchedule account; Zapier connects with a per-calendar API key; outbound webhooks carry a Verify-Token header.\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  surface: MCP server (https://platform.coschedule.com/mcp)\n  authorization_server: https://accounts-billing.coschedule.com\n  bearer_methods: [header]\n  scopes_supported: [openid]\n  evidence: https://platform.coschedule.com/.well-known/oauth-protected-resource/mcp\n  docs_quote: You sign in with your own CoSchedule account, and Claude sees only what that account can see.\n- name: zapier-calendar-api-key\n  type: apiKey\n  surface: Zapier connection\n  docs: https://coschedule.com/support/integrations/other-tools/connect-other-tools-with-zapier\n\
  \  docs_quote: Each calendar has its own API key. To connect several calendars, connect each one with its own key.\n- name: webhook-verify-token\n  type: apiKey\n  in: header\n  header: Verify-Token\n  surface: outbound webhooks (CoSchedule to your endpoint)\n  docs: https://coschedule.com/support/integrations/other-tools/use-webhooks\n  docs_quote: CoSchedule sends the token in a Verify-Token header with every call, so your endpoint can check that the call came from CoSchedule.\n"
source_yaml_url: https://artifacts.apis.io/coschedule-com/authentication/coschedule-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Marketing
- Social Media Management
- Content Calendar
- Marketing Automation
- Scheduling
- MCP
---
