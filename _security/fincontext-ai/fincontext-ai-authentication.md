---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FinContext Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinContext declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FinContext
provider_slug: fincontext-ai
scheme_count: 2
schemes:
- description: Per-user API token minted by POST /api/agent-signup (new users) or POST /api/agent-login (existing users). Sent as a Bearer token in the Authorization header on MCP calls to https://fincontext.ai/mcp. Tokens are prefixed `fc_`. Each login mints a new token; the optional agent_name field labels the token so users can audit and revoke individual agent sessions from the token-management page.
  endpoint: https://fincontext.ai/mcp
  name: API token (Bearer)
  scheme: bearer
  type: http
- description: FinContext also supports an OAuth Connector flow using the authorization_code grant at POST /oauth/token. Both this flow and the API-token flow trigger a security-notification email to the account owner on each successful sign-in (agent/client name, timestamp, IP, device, revocation link).
  flows:
    authorization_code:
      token_url: https://fincontext.ai/oauth/token
  name: OAuth Connector flow
  type: oauth2
slug: fincontext-ai-authentication
source_filename: fincontext-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://fincontext.ai/llms-full.txt
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fincontext.ai/llms-full.txt\nsources:\n- https://fincontext.ai/llms-full.txt\n- https://fincontext.ai/llms.txt\ndocs: https://fincontext.ai/llms-full.txt\nschemes:\n- type: http\n  scheme: bearer\n  name: API token (Bearer)\n  description: Per-user API token minted by POST /api/agent-signup (new users) or POST /api/agent-login (existing users). Sent as a Bearer token in the Authorization header on MCP calls to https://fincontext.ai/mcp. Tokens are prefixed `fc_`. Each login mints a new token; the optional agent_name field labels the token so users can audit and revoke individual agent sessions from the token-management page.\n  endpoint: https://fincontext.ai/mcp\n- type: oauth2\n  name: OAuth Connector flow\n  description: FinContext also supports an OAuth Connector flow using the authorization_code grant at POST /oauth/token. Both this flow and the API-token flow trigger a security-notification email to the account\
  \ owner on each successful sign-in (agent/client name, timestamp, IP, device, revocation link).\n  flows:\n    authorization_code:\n      token_url: https://fincontext.ai/oauth/token\nnotes: |\n  Bank-account access is itself brokered by Plaid using read-only OAuth: FinContext never sees banking credentials, and Plaid access tokens are encrypted at the application level before storage.\n"
source_yaml_url: https://artifacts.apis.io/fincontext-ai/authentication/fincontext-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- MCP
- Artificial Intelligence
- Personal Finance
- Banking
- Plaid
- Fintech
- Read Only
---
