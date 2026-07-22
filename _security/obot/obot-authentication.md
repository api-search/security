---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Obot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obot secures its APIs with oauth2 and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Obot
provider_slug: obot
scheme_count: 0
schemes: []
slug: obot-authentication
source_filename: obot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.obot.ai/configuration/auth-providers/\ndocs: https://docs.obot.ai/configuration/auth-providers/\nsummary:\n  types: [oauth2, openIdConnect]\n  model: >-\n    Obot authenticates users via external OAuth/OIDC identity providers and\n    issues platform API tokens (unified API-key model since v0.23.0) for\n    connecting through the MCP gateway. MCP servers behind the gateway are\n    fronted by OAuth 2.1 (mcp-oauth-proxy) with Dynamic Client Registration and\n    consent screens.\nidentity_providers:\n  - name: Google\n    tier: open-source\n  - name: GitHub\n    tier: open-source\n  - name: Okta\n    tier: enterprise\n  - name: Microsoft Entra ID\n    tier: enterprise\napi_tokens:\n  since: v0.23.0\n  note: A single API-key model covers connecting to and through the gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obot/refs/heads/main/authentication/obot-authentication.yml
summary_line: oauth2/openIdConnect · 0 schemes
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- MCP Gateway
- Open Source
- Agent Governance
- Access Control
- Developer Tools
---
