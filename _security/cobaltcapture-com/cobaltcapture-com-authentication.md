---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cobalt Capture Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobalt Capture declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cobalt Capture
provider_slug: cobaltcapture-com
scheme_count: 4
schemes:
- description: 'The anonymous MCP endpoint "needs no sign-in: your agent''s reviews start out anonymous, and you save each one to your account afterwards." Reads are public: "no auth, the same access as opening the link in a browser." The provider notes "Cobalt serves POST-only Streamable HTTP and publishes no OAuth discovery".'
  endpoint: https://cobaltcapture.com/mcp
  name: anonymous
  type: none
- description: 'Connecting /mcp/account requires signing in to Cobalt once (in Claude Code: run /mcp, pick cobalt and choose Authenticate); every review the agent makes then goes into the account. The underlying mechanism is not documented.'
  endpoint: https://cobaltcapture.com/mcp/account
  name: account-sign-in
  type: interactive-sign-in
- description: create_review returns a review link and a token; the agent passes that token as claim_token to add_screenshot / add_note / update_review. Once a review is saved to an account, the owner generates a per-review token via Export & more -> Hand to your agent; generating again rotates the token and Revoke ends access.
  name: claim_token
  type: per-resource-token
- description: create_inbox returns an address and an inbox_token; only the holder of an inbox's inbox_token can read it.
  name: inbox_token
  type: per-resource-token
slug: cobaltcapture-com-authentication
source_filename: cobaltcapture-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cobaltcapture.com/developers\ndocs: https://cobaltcapture.com/developers\nschemes:\n- name: anonymous\n  type: none\n  endpoint: https://cobaltcapture.com/mcp\n  description: 'The anonymous MCP endpoint \"needs no sign-in: your agent''s reviews start out anonymous, and you save each one to your account afterwards.\" Reads are public: \"no auth, the same access as opening the link in a browser.\" The provider notes \"Cobalt serves POST-only Streamable HTTP and publishes no OAuth discovery\".'\n- name: account-sign-in\n  type: interactive-sign-in\n  endpoint: https://cobaltcapture.com/mcp/account\n  description: 'Connecting /mcp/account requires signing in to Cobalt once (in Claude Code: run /mcp, pick cobalt and choose Authenticate); every review the agent makes then goes into the account. The underlying mechanism is not documented.'\n- name: claim_token\n  type: per-resource-token\n  description: create_review returns\
  \ a review link and a token; the agent passes that token as claim_token to add_screenshot / add_note / update_review. Once a review is saved to an account, the owner generates a per-review token via Export & more -> Hand to your agent; generating again rotates the token and Revoke ends access.\n- name: inbox_token\n  type: per-resource-token\n  description: create_inbox returns an address and an inbox_token; only the holder of an inbox's inbox_token can read it.\n"
source_yaml_url: https://artifacts.apis.io/cobaltcapture-com/authentication/cobaltcapture-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Visual Feedback
- Screenshots
- Usability Testing
- Website Review
- AI Agents
- MCP
- Pricing Teardown
---
