---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cequence Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cequence Security declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cequence Security
provider_slug: cequence-security
scheme_count: 0
schemes: []
slug: cequence-security-authentication
source_filename: cequence-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.aigateway.cequence.ai/docs/guides/multi-authentication\ndocs:\n- https://docs.aigateway.cequence.ai/docs/guides/multi-authentication\n- https://docs.aigateway.cequence.ai/docs/sso-mcp\n- https://docs.aigateway.cequence.ai/docs/remote-mcp-servers/cequence-ai-gateway\nsummary: >-\n  Cequence AI Gateway is a two-sided authentication broker. Inbound (\"agent authentication\") governs how\n  an AI client proves identity to a gateway-published MCP server; outbound (\"app authentication\")\n  governs the credential the gateway injects when calling the upstream API or MCP server. Agents never\n  hold the upstream credential — \"Agents never see your API keys or tokens. The gateway injects them on\n  the way out.\"\ninbound:\n  description: Agent -> Cequence AI Gateway\n  schemes:\n  - id: sso-interactive\n    type: openIdConnect\n    description: >-\n      \"When a user connects, they'll see a familiar SSO login prompt\
  \ in their browser.\" Intended for\n      team members using AI coding assistants such as Cursor or Claude Desktop.\n    identity_providers:\n    - {name: Microsoft Entra ID, docs: https://docs.aigateway.cequence.ai/docs/sso-mcp/microsoft-entra}\n    - {name: Microsoft Entra Proxy, docs: https://docs.aigateway.cequence.ai/docs/sso-mcp/microsoft-entra-proxy}\n    - {name: Google Workspace, docs: https://docs.aigateway.cequence.ai/docs/sso-mcp/google-workspace}\n    - {name: Okta, docs: https://docs.aigateway.cequence.ai/docs/sso-mcp/okta}\n    - {name: GitLab, docs: https://docs.aigateway.cequence.ai/docs/sso-mcp/gitlab-sso-configuration}\n    group_mapping: SSO groups map to Teams, which gate access to MCP servers and Agent Personas.\n  - id: passthrough\n    type: http\n    description: Forwards caller credentials as-is, optionally with JWT validation — \"the gateway checks the token before forwarding the request.\"\n  - id: access-key\n    type: apiKey\n    description: Agent Personas\
  \ support access-key authentication in addition to SSO.\n  - id: api-key\n    type: apiKey\n    description: API key inbound authentication is offered on registered APIs (API Registry).\n  - id: bearer\n    type: http\n    scheme: bearer\n  - id: basic\n    type: http\n    scheme: basic\n  - id: jwt-bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\noutbound:\n  description: Cequence AI Gateway -> upstream API / remote MCP server\n  schemes:\n  - id: oauth2-authorization\n    type: oauth2\n    flow: authorizationCode\n    version: OAuth 2.1\n    description: >-\n      \"the most common setup for apps like Gmail, Google Drive, Slack, or GitLab\" — user-consent\n      authorization-code flow.\n  - id: oauth2-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    version: OAuth 2.1\n    description: Service accounts; the gateway holds a fixed credential set.\n    configuration: [token_url, client_id, client_secret, scopes]\n  - id: api-key\n    type: apiKey\n\
  \    in: [header, query]\n    configuration: [key_name, key_value, location]\n  - id: bearer\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <token>'\n  - id: jwt-bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: '\"self-contained JWT (JSON Web Token) with embedded claims and a digital signature\"'\n  - id: basic\n    type: http\n    scheme: basic\n  - id: passthrough\n    type: none\n    description: No added credential; the caller-provided authentication is forwarded unchanged.\n  additional_headers:\n    supported: true\n    kinds: [oauth2 service tokens, forwarded caller tokens, token exchange, stored API keys, caller identity headers, custom headers]\nfirst_party_mcp_server:\n  auth: OAuth 2.0 / OIDC, browser-based authorization-code flow with public-client PKCE\n  identity_provider: Descope\n  see: mcp/cequence-security-mcp.yml\nscopes:\n  provider_scope_registry_published: false\n  note: >-\n    Cequence does not publish\
  \ an OAuth scope registry of its own — scopes configured in the gateway are\n    the UPSTREAM provider's scopes (e.g. the documented Atlassian OAuth scope guide at\n    /docs/guides/atlassian-oauth-scopes). No scopes/ artifact is emitted for that reason.\nenforcement_order: >-\n  Routing (404) -> Authentication (401) -> Authorization (403) -> Rate limiting (429) -> Security\n  interceptors, DLP and behavioral rules -> Upstream call (502/503).\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - url: https://docs.aigateway.cequence.ai/docs/guides/multi-authentication\n    http_status: 200\n  - url: https://docs.aigateway.cequence.ai/docs/guides/security-policies\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence-security/refs/heads/main/authentication/cequence-security-authentication.yml
summary_line: 0 schemes
tags:
- API Security
- AI Gateway
- MCP
- Agentic AI
- Bot Management
- API Discovery
- API Governance
- Fraud Detection
- WAAP
- Cybersecurity
- API Testing
- agent-native
---
