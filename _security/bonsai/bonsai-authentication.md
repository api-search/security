---
api_key_in: []
auth_types:
- oauth2
description: Bonsai's programmatic surface (its hosted MCP server) authenticates with OAuth 2.1 authorization-code flow using PKCE, driven by the AI client. There are no API keys to create or paste; on first call the user is directed to Bonsai to log in, approves in the browser, and the client receives a short-lived token (~15 minutes, auto-refreshed) that is passed through to Bonsai without being stored by the MCP server. Access is scoped to the user's existing Bonsai role.
kind: authentication
layout: security
method: searched
name: Bonsai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bonsai secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bonsai
provider_slug: bonsai
scheme_count: 1
schemes:
- flows:
  - description: OAuth 2.1 authorization-code flow with PKCE, brokered by the AI client against Bonsai; MCP server passes the bearer token through without storage.
    flow: authorizationCode
    pkce: true
    token_ttl_seconds: 900
  name: oauth2-pkce
  sources:
  - https://docs.hellobonsai.com/
  - mcp/bonsai-mcp.yml
  type: oauth2
slug: bonsai-authentication
source_filename: bonsai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.hellobonsai.com/\ndocs: https://docs.hellobonsai.com/\ndescription: >-\n  Bonsai's programmatic surface (its hosted MCP server) authenticates with\n  OAuth 2.1 authorization-code flow using PKCE, driven by the AI client. There\n  are no API keys to create or paste; on first call the user is directed to Bonsai\n  to log in, approves in the browser, and the client receives a short-lived token\n  (~15 minutes, auto-refreshed) that is passed through to Bonsai without being\n  stored by the MCP server. Access is scoped to the user's existing Bonsai role.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2-pkce\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    token_ttl_seconds: 900\n    description: >-\n      OAuth 2.1 authorization-code flow with PKCE, brokered by the AI client\n      against Bonsai; MCP server passes the bearer token through without\
  \ storage.\n  sources:\n  - https://docs.hellobonsai.com/\n  - mcp/bonsai-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai/refs/heads/main/authentication/bonsai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- B2B
- Business Management
- Freelancing
- Agencies
- CRM
- Project Management
- Time Tracking
- Invoicing
- Proposals
- Contracts
- Accounting
- MCP
---
