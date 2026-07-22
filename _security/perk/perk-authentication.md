---
api_key_in: []
auth_types: []
description: Perk supports two authentication styles. Customers accessing their own data use an account-admin API key. Partners building integrations on behalf of customers use OAuth 2.0 Authorization Code. The MCP server uses OAuth 2.0 Authorization Code with PKCE and Dynamic Client Registration.
kind: authentication
layout: security
method: searched
name: Perk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perk declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Perk
provider_slug: perk
scheme_count: 3
schemes:
- audience: Perk customers accessing their own data
  companion_header:
    name: Api-Version
    value: '1'
  format: apikey <your_api_key>
  id: api_key
  in: header
  managed_in: Settings > Developer > API tools
  name: Authorization
  scope_note: An API key has the same access rights as an account admin.
  type: apiKey
- access_token_lifetime: 1 hour
  audience: Partners integrating on behalf of customers
  flow: authorization_code
  id: oauth2
  refresh_policy: refresh-and-rotate; every token call returns a new access+refresh pair; 2-minute grace period for retries
  refresh_token_lifetime: 30 days (rotating; old refresh token revoked 2 minutes after use)
  type: oauth2
- audience: MCP AI clients
  authorization_server: https://mcp.perk.com/api/mcp
  dynamic_client_registration: true
  flow: authorization_code
  id: oauth2_pkce
  pkce: true
  scopes:
  - user:read
  - trip:read
  - expenses:read
  - report:write
  - my-travel-policy:read
  type: oauth2
slug: perk-authentication
source_filename: perk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.perk.com/docs/quickstart.md\ndocs: https://developers.perk.com/reference/oauth-20-implementation-guidance\nname: Perk API Authentication\ntype: Authentication\ndescription: >-\n  Perk supports two authentication styles. Customers accessing their own data use an\n  account-admin API key. Partners building integrations on behalf of customers use\n  OAuth 2.0 Authorization Code. The MCP server uses OAuth 2.0 Authorization Code with\n  PKCE and Dynamic Client Registration.\nschemes:\n- id: api_key\n  type: apiKey\n  in: header\n  name: Authorization\n  format: \"apikey <your_api_key>\"\n  audience: Perk customers accessing their own data\n  scope_note: An API key has the same access rights as an account admin.\n  managed_in: Settings > Developer > API tools\n  companion_header:\n    name: Api-Version\n    value: '1'\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  audience: Partners integrating on\
  \ behalf of customers\n  access_token_lifetime: 1 hour\n  refresh_token_lifetime: 30 days (rotating; old refresh token revoked 2 minutes after use)\n  refresh_policy: refresh-and-rotate; every token call returns a new access+refresh pair; 2-minute grace period for retries\n- id: oauth2_pkce\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  dynamic_client_registration: true   # RFC 7591\n  audience: MCP AI clients\n  authorization_server: https://mcp.perk.com/api/mcp\n  scopes:\n  - user:read\n  - trip:read\n  - expenses:read\n  - report:write\n  - my-travel-policy:read\nscim:\n  note: The SCIM provisioning API authenticates with a bearer token issued in Perk's SCIM setup.\n  base: https://app.perk.com/api/v2/scim\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/authentication/perk-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Corporate Travel
- Expense Management
- Spend Management
- Travel
- Invoices
- Fintech
- SaaS
---
