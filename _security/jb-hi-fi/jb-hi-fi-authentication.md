---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Jb Hi Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: JB Hi-Fi declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: JB Hi-Fi
provider_slug: jb-hi-fi
scheme_count: 3
schemes:
- description: Required "Agent profile URI for UCP discovery." on all 13 tools.
  in: tool-arguments
  name: meta.ucp-agent.profile
  type: agent-profile
- description: '"Server-to-server requests and hosted or remote browsers must use Web Bot Auth and follow the service''s authentication requirements."'
  docs: https://shopify.dev/docs/api/storefront#identifying-bots-with-web-bot-auth
  name: Web Bot Auth
  type: http-message-signatures
- auth_url: https://accounts.shop.app
  description: UCP dev.ucp.common.identity_linking capability; scopes object is empty in the profile.
  name: identity_linking (app.shop.accounts)
  type: oauth2
slug: jb-hi-fi-authentication
source_filename: jb-hi-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource:\n- https://www.jbhifi.com.au/agents.md\n- https://www.jbhifi.com.au/.well-known/ucp\ndocs: https://www.jbhifi.com.au/agents.md\nsummary: No OpenAPI and no API keys. The UCP shopping MCP service identifies agents by a UCP agent profile URI passed in every tool call's meta, and agents.md requires Web Bot Auth for server-to-server and hosted-browser traffic. Buyer account linking is OAuth2 through Shop accounts as declared in the UCP profile. The preflight also recorded a /.well-known/oauth-protected-resource document on www.jbhifi.com.au.\nschemes:\n- type: agent-profile\n  name: meta.ucp-agent.profile\n  in: tool-arguments\n  description: Required \"Agent profile URI for UCP discovery.\" on all 13 tools.\n- type: http-message-signatures\n  name: Web Bot Auth\n  description: '\"Server-to-server requests and hosted or remote browsers must use Web Bot Auth and follow the service''s authentication requirements.\"'\n  docs: https://shopify.dev/docs/api/storefront#identifying-bots-with-web-bot-auth\n\
  - type: oauth2\n  name: identity_linking (app.shop.accounts)\n  auth_url: https://accounts.shop.app\n  description: UCP dev.ucp.common.identity_linking capability; scopes object is empty in the profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jb-hi-fi/refs/heads/main/authentication/jb-hi-fi-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Retail
- Consumer Electronics
- E-Commerce
- Home Entertainment
- Australia
- Agentic Commerce
---
