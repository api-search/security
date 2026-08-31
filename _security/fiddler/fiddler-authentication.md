---
api_key_in: []
auth_types: []
description: Authentication profile for the Fiddler programmatic surface. Fiddler publishes no OpenAPI, so nothing here is derived from securitySchemes — every scheme below was read from the provider's own documentation or probed from a live /.well-known/ document.
kind: authentication
layout: security
method: searched
name: Fiddler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiddler declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fiddler
provider_slug: fiddler
scheme_count: 3
schemes:
- additional_gates:
  - The user must be signed in to Fiddler Everywhere (is_user_logged_in / initiate_login).
  - The Fiddler root certificate must be trusted for HTTPS interception.
  - An administrator can disable the server entirely via the DisableMCP policy key.
  docs: https://www.telerik.com/fiddler/fiddler-everywhere/documentation/agent-tools/fiddler-mcp-server
  entitlement: Requires a Fiddler Everywhere Pro or higher subscription.
  example: 'Authorization: ApiKey <key>'
  header: Authorization
  id: mcp-api-key
  in: header
  issuance: Generated inside the Fiddler Everywhere desktop application at Settings > MCP Server. As of Fiddler Everywhere 7.7.2 (2026-03-26) the app exposes an internal API endpoint for MCP API key generation.
  name: Fiddler MCP Server API Key
  rotation: Regenerate from Settings > MCP Server. No published rotation policy or expiry.
  scheme_prefix: ApiKey
  surface: http://localhost:8868/mcp
  type: apiKey
- authorization_endpoint: https://www.telerik.com/sitefinity/oauth/authorize
  discovery: https://www.telerik.com/.well-known/oauth-authorization-server
  flows:
  - authorization_code
  - refresh_token
  id: telerik-identity-oauth2
  issuer: https://www.telerik.com
  method: probed
  name: Telerik Identity (telerik.com website OAuth 2.0)
  ownership_note: This is the Sitefinity-backed Telerik Identity used to sign in to telerik.com (accounts, licences, downloads, support). It is NOT an authorization server for a Fiddler product API; Fiddler's own agent surface uses the API-key scheme above.
  pkce: S256
  scope_note: The metadata document advertises no scopes_supported, so no scopes/ artifact is emitted — there is nothing to enumerate.
  scopes_supported: []
  status: 200
  token_endpoint: https://www.telerik.com/sitefinity/oauth/token
  type: oauth2
- description: The desktop app authenticates the user through a browser window (initiate_login opens a Chrome window). The MCP tools is_user_logged_in and initiate_login expose this state to an agent, but the agent cannot supply credentials itself — a human completes the flow.
  id: fiddler-account-login
  name: Fiddler Everywhere application sign-in
  sso: SAML/SSO is an Enterprise-tier feature per the pricing page.
  surface: desktop application
  type: interactive
slug: fiddler-authentication
source_filename: fiddler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.telerik.com/fiddler/fiddler-everywhere/documentation/agent-tools/fiddler-mcp-server\nprovider: Fiddler\nproviderId: fiddler\ndescription: >-\n  Authentication profile for the Fiddler programmatic surface. Fiddler publishes\n  no OpenAPI, so nothing here is derived from securitySchemes — every scheme\n  below was read from the provider's own documentation or probed from a live\n  /.well-known/ document.\nschemes:\n  - id: mcp-api-key\n    name: Fiddler MCP Server API Key\n    type: apiKey\n    in: header\n    header: Authorization\n    scheme_prefix: ApiKey\n    example: 'Authorization: ApiKey <key>'\n    surface: http://localhost:8868/mcp\n    issuance: >-\n      Generated inside the Fiddler Everywhere desktop application at\n      Settings > MCP Server. As of Fiddler Everywhere 7.7.2 (2026-03-26) the app\n      exposes an internal API endpoint for MCP API key generation.\n    rotation: Regenerate from Settings\
  \ > MCP Server. No published rotation policy or expiry.\n    entitlement: Requires a Fiddler Everywhere Pro or higher subscription.\n    additional_gates:\n      - The user must be signed in to Fiddler Everywhere (is_user_logged_in / initiate_login).\n      - The Fiddler root certificate must be trusted for HTTPS interception.\n      - An administrator can disable the server entirely via the DisableMCP policy key.\n    docs: https://www.telerik.com/fiddler/fiddler-everywhere/documentation/agent-tools/fiddler-mcp-server\n  - id: telerik-identity-oauth2\n    name: Telerik Identity (telerik.com website OAuth 2.0)\n    type: oauth2\n    flows:\n      - authorization_code\n      - refresh_token\n    issuer: https://www.telerik.com\n    authorization_endpoint: https://www.telerik.com/sitefinity/oauth/authorize\n    token_endpoint: https://www.telerik.com/sitefinity/oauth/token\n    pkce: S256\n    scopes_supported: []\n    discovery: https://www.telerik.com/.well-known/oauth-authorization-server\n\
  \    method: probed\n    status: 200\n    scope_note: >-\n      The metadata document advertises no scopes_supported, so no scopes/\n      artifact is emitted — there is nothing to enumerate.\n    ownership_note: >-\n      This is the Sitefinity-backed Telerik Identity used to sign in to\n      telerik.com (accounts, licences, downloads, support). It is NOT an\n      authorization server for a Fiddler product API; Fiddler's own agent surface\n      uses the API-key scheme above.\n  - id: fiddler-account-login\n    name: Fiddler Everywhere application sign-in\n    type: interactive\n    surface: desktop application\n    description: >-\n      The desktop app authenticates the user through a browser window\n      (initiate_login opens a Chrome window). The MCP tools is_user_logged_in and\n      initiate_login expose this state to an agent, but the agent cannot supply\n      credentials itself — a human completes the flow.\n    sso: SAML/SSO is an Enterprise-tier feature per the pricing page.\n\
  no_openapi: true\nno_openapi_note: >-\n  Contract discovery on 2026-08-29 probed /openapi.json, /swagger.json and\n  /api-docs on www.telerik.com and docs.telerik.com (all 404) and api.telerik.com\n  (does not resolve). Fiddler publishes no REST contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiddler/refs/heads/main/authentication/fiddler-authentication.yml
summary_line: 3 schemes
tags:
- API Debugging
- HTTP Debugging
- HTTP Proxy
- Performance Testing
- Traffic Inspection
- Web Development
- Developer Tools
- Model Context Protocol
- Agent Tooling
---
