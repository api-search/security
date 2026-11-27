---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cookie Compliance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cookie Compliance declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cookie Compliance
provider_slug: cookie-compliance-co
scheme_count: 3
schemes:
- applies_to: https://mcp.cookie-compliance.co/mcp/account
  authorization_server_metadata: https://mcp.cookie-compliance.co/.well-known/oauth-authorization-server
  description: OAuth 2.1 (MCP authorization), dynamic client registration, PKCE required. The client asks the customer to sign in when the server is added; a Cookie Compliance page opens in the browser to approve.
  name: oauth2-mcp
  protected_resource_metadata: https://mcp.cookie-compliance.co/.well-known/oauth-protected-resource/mcp/account
  scopes:
  - banner:read
  - banner:write
  - offline_access
  token_lifetime: a signed-in connection renews while it is used, though the client may occasionally ask the customer to sign in again
  type: oauth2
- applies_to: https://mcp.cookie-compliance.co/mcp/account
  description: 'Fallback for clients with no sign-in. A token is a long code that starts with hu_, created by an Admin or Super Admin at https://app.hu-manity.co/#/api-tokens/new (the dashboard calls this Temporary Login) and sent as "Authorization: Bearer hu_…" in the client''s connection settings. A Master Admin sign-in cannot create one.'
  expiry: 'Manual: "Expires At: pick the latest date the date picker allows (up to 30 days ahead)". Server metadata: "A pasted token expires (at most 90 days) and cannot be renewed". Tokens can be revoked from the same list (Revoke Token).'
  header: Authorization
  name: api-token
  prefix: hu_
  scheme: bearer
  type: http
- applies_to: https://mcp.cookie-compliance.co/mcp
  description: No signup, no API key and no card for the try-it-out address.
  name: anonymous
  type: none
slug: cookie-compliance-co-authentication
source_filename: cookie-compliance-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://manual.hu-manity.co/connect/\ndocs: https://manual.hu-manity.co/connect/\nname: Cookie Compliance authentication\nnote: Cookie Compliance has no public REST API; authentication applies to its MCP server. https://mcp.cookie-compliance.co/mcp is anonymous (demo, install and help tools); https://mcp.cookie-compliance.co/mcp/account requires sign-in. Auth details also come from the server's own landing metadata (examples/cookie-compliance-co-mcp-landing-metadata.json, GET https://mcp.cookie-compliance.co/).\nschemes:\n- name: oauth2-mcp\n  type: oauth2\n  description: 'OAuth 2.1 (MCP authorization), dynamic client registration, PKCE required. The client asks the customer to sign in when the server is added; a Cookie Compliance page opens in the browser to approve.'\n  applies_to: https://mcp.cookie-compliance.co/mcp/account\n  protected_resource_metadata: https://mcp.cookie-compliance.co/.well-known/oauth-protected-resource/mcp/account\n\
  \  authorization_server_metadata: https://mcp.cookie-compliance.co/.well-known/oauth-authorization-server\n  scopes: [banner:read, banner:write, offline_access]\n  token_lifetime: a signed-in connection renews while it is used, though the client may occasionally ask the customer to sign in again\n- name: api-token\n  type: http\n  scheme: bearer\n  description: 'Fallback for clients with no sign-in. A token is a long code that starts with hu_, created by an Admin or Super Admin at https://app.hu-manity.co/#/api-tokens/new (the dashboard calls this Temporary Login) and sent as \"Authorization: Bearer hu_…\" in the client''s connection settings. A Master Admin sign-in cannot create one.'\n  prefix: hu_\n  header: Authorization\n  applies_to: https://mcp.cookie-compliance.co/mcp/account\n  expiry: 'Manual: \"Expires At: pick the latest date the date picker allows (up to 30 days ahead)\". Server metadata: \"A pasted token expires (at most 90 days) and cannot be renewed\". Tokens can be revoked\
  \ from the same list (Revoke Token).'\n- name: anonymous\n  type: none\n  description: No signup, no API key and no card for the try-it-out address.\n  applies_to: https://mcp.cookie-compliance.co/mcp\n"
source_yaml_url: https://artifacts.apis.io/cookie-compliance-co/authentication/cookie-compliance-co-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cookie Consent
- Consent Management
- Privacy
- GDPR
- CCPA
- Compliance
- MCP
---
