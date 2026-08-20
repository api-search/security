---
api_key_in:
- header
- query
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Woowup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
overview: WoowUp secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and implicit flow(s).
provider_name: WoowUp
provider_slug: woowup
scheme_count: 3
schemes:
- format: 'Authorization: Basic {apikey}'
  in: header
  name: apikeyHeader
  notes: 'The docs'' recommended method sends the raw account API key after the Basic keyword (not base64 user:pass). Rate-limiting code examples also show ''Authorization: Bearer {api_token}'' accepted.'
  parameter: Authorization
  recommended: true
  type: apiKey
- format: ?apikey={apikey}
  in: query
  name: apikeyQuery
  parameter: apikey
  recommended: false
  type: apiKey
- authorization_server_metadata: https://mcp.woowup.com/.well-known/oauth-authorization-server
  detail: scopes/woowup-scopes.yml
  dynamic_client_registration: https://mcp.woowup.com/oauth/register
  format: 'Authorization: Bearer {access_token}'
  in: header
  issuer: https://my-dev-instance-ap11e0.us1.zitadel.cloud
  name: MCPOAuth2
  notes: Applies to the hosted MCP server only, not to REST API v3. An unauthenticated request returns HTTP 401 with an RFC 6750 WWW-Authenticate Bearer challenge naming the resource-metadata URL. This OAuth surface is not mentioned anywhere in the WoowUp developer docs; it was found by probing.
  parameter: Authorization
  pkce:
  - S256
  protected_resource_metadata: https://mcp.woowup.com/.well-known/oauth-protected-resource
  scopes:
  - openid
  - profile
  - email
  - campaigns:read
  surface: https://mcp.woowup.com/mcp
  type: oauth2
slug: woowup-authentication
source_filename: woowup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://woowup-docs.gitbook.io/woowup-developer-docs/master#authentication\nsource: >-\n  https://woowup-docs.gitbook.io/woowup-developer-docs/master (Getting Started,\n  Authentication section) and connection-security page. WoowUp publishes no\n  OpenAPI, so this profile is captured from the docs rather than derived from\n  securitySchemes. The oauth2 scheme below was added 2026-08-13 from live\n  probes of https://mcp.woowup.com/.well-known/oauth-protected-resource and\n  /.well-known/oauth-authorization-server (both HTTP 200, saved verbatim under\n  well-known/).\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, implicit]\n  surfaces:\n    rest_api_v3: apiKey only — no OAuth, no scopes\n    mcp_server: oauth2 only — no API key accepted\nschemes:\n  - name: apikeyHeader\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format:\
  \ 'Authorization: Basic {apikey}'\n    recommended: true\n    notes: >-\n      The docs' recommended method sends the raw account API key after the\n      Basic keyword (not base64 user:pass). Rate-limiting code examples also\n      show 'Authorization: Bearer {api_token}' accepted.\n  - name: apikeyQuery\n    type: apiKey\n    in: query\n    parameter: apikey\n    format: '?apikey={apikey}'\n    recommended: false\n  - name: MCPOAuth2\n    type: oauth2\n    surface: https://mcp.woowup.com/mcp\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Bearer {access_token}'\n    issuer: https://my-dev-instance-ap11e0.us1.zitadel.cloud\n    protected_resource_metadata: https://mcp.woowup.com/.well-known/oauth-protected-resource\n    authorization_server_metadata: https://mcp.woowup.com/.well-known/oauth-authorization-server\n    dynamic_client_registration: https://mcp.woowup.com/oauth/register\n    pkce: [S256]\n    scopes: [openid, profile, email, 'campaigns:read']\n \
  \   detail: scopes/woowup-scopes.yml\n    notes: >-\n      Applies to the hosted MCP server only, not to REST API v3. An\n      unauthenticated request returns HTTP 401 with an RFC 6750\n      WWW-Authenticate Bearer challenge naming the resource-metadata URL. This\n      OAuth surface is not mentioned anywhere in the WoowUp developer docs; it\n      was found by probing.\nkey_management:\n  issuance: Log into WoowUp and get the API key from the Configuration / My Account section (app.woowup.com).\n  revocation: >-\n    Requests from deleted accounts receive HTTP 410 Gone with code\n    account_deleted; a deactivated account's API key is permanently invalid.\ntransport:\n  https_only: true\n  tls_minimum: '1.2'\n  docs: https://woowup-docs.gitbook.io/woowup-developer-docs/connection-security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woowup/refs/heads/main/authentication/woowup-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- CRM
- Loyalty
- Customer Data
- Marketing Automation
- Retail
- E-Commerce
- Push Notifications
---
