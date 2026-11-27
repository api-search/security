---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: /call-me Authentication
name_suffix: Authentication
oauth_flows: []
overview: /call-me declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: /call-me
provider_slug: callmemcp-com
scheme_count: 2
schemes:
- applies_to:
  - https://callmemcp.com/mcp
  - https://callmemcp.com/ring
  - https://callmemcp.com/text
  evidence: One server, every MCP client — no API key, no OAuth
  name: unauthenticated
  type: none
- applies_to:
  - /aiphone/calls/{call_id}/say
  - /aiphone/calls/{call_id}/hangup
  - /aiphone/sessions/label
  - /aiphone/sessions/events
  evidence: Both responses hand back a session_token, and that is a real session
  in: body (query for /aiphone/sessions/events)
  name: session_token
  note: Issued by /ring or /text, not by a login. The README says it is derived from to + from + the caller's IP.
  type: session-token
slug: callmemcp-com-authentication
source_filename: callmemcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://github.com/radres/call-me/blob/main/README.md\ndocs: https://github.com/radres/call-me/blob/main/README.md\nschemes:\n- type: none\n  name: unauthenticated\n  applies_to: [https://callmemcp.com/mcp, https://callmemcp.com/ring, https://callmemcp.com/text]\n  evidence: One server, every MCP client — no API key, no OAuth\n- type: session-token\n  name: session_token\n  in: body (query for /aiphone/sessions/events)\n  applies_to: ['/aiphone/calls/{call_id}/say', '/aiphone/calls/{call_id}/hangup', /aiphone/sessions/label, /aiphone/sessions/events]\n  evidence: Both responses hand back a session_token, and that is a real session\n  note: Issued by /ring or /text, not by a login. The README says it is derived from to + from + the caller's IP.\nsummary: No authentication scheme. The README states \"One server, every MCP client — no API key, no OAuth\" for https://callmemcp.com/mcp, and the plain HTTP endpoints (/ring, /text)\
  \ are described as \"No MCP client, no plugin, no token.\"\nnote: >-\n  The only addressing credential is the user's 10-digit /call-me number (obtained in the\n  iOS/Android app). /ring and /text return a session_token that the README says \"is derived\n  from to + from + your IP\" and is reused for /aiphone/calls/{call_id}/say, /hangup,\n  /aiphone/sessions/label and /aiphone/sessions/events. The CLI treats session tokens and the\n  paired number as credentials (umask 077). Access to the service is a subscription started in\n  the mobile app, not an API key.\n"
source_yaml_url: https://artifacts.apis.io/callmemcp-com/authentication/callmemcp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- MCP
- AI Agents
- Voice
- Phone Calls
- Notification
- Mobile
- Developer Tools
---
