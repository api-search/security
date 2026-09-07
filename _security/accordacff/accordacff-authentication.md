---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accordacff Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accord declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Accord
provider_slug: accordacff
scheme_count: 2
schemes:
- applies_to: https://api2.inaccord.com/graphql
  entitlement: Requires an Accord license that includes API access. Accord's pricing page lists "API Support" only under the Enterprise tier.
  expiry: not documented
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  id: api-key-bearer
  issuance: Created in the Accord app under Settings → Workspace → API Keys by a workspace admin only. Accord states the key is shown once — "Copy immediately after creation".
  rotation: '"To rotate a key without downtime, create the replacement first, switch your client to the new key, then delete the old one." Accord exposes createApiKey / deleteApiKey mutations in the GraphQL reference.'
  scheme: bearer
  scopes: none — the API key has no scope surface; authorization is row-level security, not scopes
  scoping: '"A key acts within the workspace it was created in. The same Row-Level Security rules that apply to in-app sessions apply to API key requests — a key cannot read or change data its workspace wouldn''t otherwise be able to."'
  source: https://developers.inaccord.com/authentication
  type: http
- applies_to: https://api.inaccord.com/1/mcp/mcp
  authorization_endpoint: https://api.inaccord.com/1/mcp/authorize
  bearer_methods:
  - header
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2-pkce-mcp
  issuer: https://api.inaccord.com
  registration_endpoint: https://api.inaccord.com/1/mcp/register
  scopes:
  - mcp:read
  - mcp:write
  source: https://api.inaccord.com/.well-known/oauth-authorization-server
  spec: OAuth 2.1 with PKCE (RFC 7636 S256)
  token_endpoint: https://api.inaccord.com/1/mcp/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
  user_flow: The MCP client opens the default browser to api.inaccord.com/1/mcp/authorize, the user enters their workspace slug (e.g. acme for acme.inaccord.com) and completes Google SSO; the client stores the token. Accord states "no API keys to manage or rotate".
slug: accordacff-authentication
source_filename: accordacff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developers.inaccord.com/authentication\ndocs: https://developers.inaccord.com/authentication\nname: Accord authentication\nnote: >-\n  Accord runs two distinct authentication models on two distinct hosts: a workspace-scoped bearer API key for the\n  GraphQL Developer API on api2.inaccord.com, and OAuth 2.1 + PKCE for the MCP server on api.inaccord.com. There is\n  no OpenAPI to derive securitySchemes from; both models are read from Accord's own published documentation, and the\n  OAuth parameters are additionally confirmed against Accord's anonymous /.well-known/ metadata.\nschemes:\n  - id: api-key-bearer\n    type: http\n    scheme: bearer\n    applies_to: https://api2.inaccord.com/graphql\n    header: Authorization\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    issuance: >-\n      Created in the Accord app under Settings → Workspace → API Keys by a workspace admin only. Accord states the key\n      is shown\
  \ once — \"Copy immediately after creation\".\n    scoping: >-\n      \"A key acts within the workspace it was created in. The same Row-Level Security rules that apply to in-app\n      sessions apply to API key requests — a key cannot read or change data its workspace wouldn't otherwise be\n      able to.\"\n    rotation: >-\n      \"To rotate a key without downtime, create the replacement first, switch your client to the new key, then delete\n      the old one.\" Accord exposes createApiKey / deleteApiKey mutations in the GraphQL reference.\n    expiry: not documented\n    scopes: none — the API key has no scope surface; authorization is row-level security, not scopes\n    entitlement: >-\n      Requires an Accord license that includes API access. Accord's pricing page lists \"API Support\" only under the\n      Enterprise tier.\n    source: https://developers.inaccord.com/authentication\n  - id: oauth2-pkce-mcp\n    type: oauth2\n    spec: OAuth 2.1 with PKCE (RFC 7636 S256)\n    applies_to:\
  \ https://api.inaccord.com/1/mcp/mcp\n    issuer: https://api.inaccord.com\n    authorization_endpoint: https://api.inaccord.com/1/mcp/authorize\n    token_endpoint: https://api.inaccord.com/1/mcp/token\n    registration_endpoint: https://api.inaccord.com/1/mcp/register\n    grant_types:\n      - authorization_code\n      - refresh_token\n    token_endpoint_auth_methods:\n      - none\n    dynamic_client_registration: true\n    bearer_methods:\n      - header\n    scopes:\n      - mcp:read\n      - mcp:write\n    user_flow: >-\n      The MCP client opens the default browser to api.inaccord.com/1/mcp/authorize, the user enters their workspace\n      slug (e.g. acme for acme.inaccord.com) and completes Google SSO; the client stores the token. Accord states\n      \"no API keys to manage or rotate\".\n    source: https://api.inaccord.com/.well-known/oauth-authorization-server\nfailure_responses:\n  - http_status: 400\n    meaning: Malformed request or missing query\n  - http_status: 401\n\
  \    meaning: Missing or invalid API key\n  - http_status: 403\n    meaning: Unauthorized API key\n  - graphql_extensions_code: '42501'\n    meaning: permission denied — the key's role lacks visibility or modification rights on the relation\nsso:\n  workspace_sso: Google SSO for the MCP authorization flow\n  enterprise_sso: >-\n    Accord's pricing page lists \"Single Sign-on\" as an Enterprise-tier feature. No SAML/SCIM specification is\n    published.\nx-evidence:\n  - url: https://developers.inaccord.com/authentication\n    http_status: 200\n    fetched: '2026-09-06'\n  - url: https://api.inaccord.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-09-06'\n  - url: https://api2.inaccord.com/graphql\n    note: anonymous introspection POST\n    http_status: 401\n    fetched: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accordacff/refs/heads/main/authentication/accordacff-authentication.yml
summary_line: 2 schemes
tags:
- Sales Enablement
- Revenue Operations
- Customer Collaboration
- Sales Engagement
- Customer Onboarding
- Mutual Action Plans
- CRM
- GraphQL
- MCP
- agent-native
- SaaS
- Company
---
