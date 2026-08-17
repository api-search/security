---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Frontify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Frontify secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Frontify
provider_slug: frontify
scheme_count: 3
schemes:
- authorizationUrl: https://{instance}.frontify.com/api/oauth/authorize
  description: Interactive OAuth 2.0 authorization against a user's Frontify instance — used by the Frontify Authenticator, Finder, Brand SDK apps and custom integrations. Client ID / Client Secret are issued by creating an OAuth application in the instance's Developer settings; the scope set requested at registration must match the scope set requested at authorization.
  flow: authorizationCode
  name: OAuth2 (Authorization Code) — Frontify instance
  scopes: scopes/frontify-scopes.yml
  sources:
  - developer.frontify.com
  - '@frontify/frontify-authenticator'
  - third-party connector docs
  type: oauth2
- description: Personal / API access tokens generated per Frontify instance, sent as a Bearer token for server-to-server GraphQL calls. Frontify's knowledge base notes API access must be enabled on the account.
  format: Bearer <token>
  in: header
  name: API Token (Bearer) — Frontify instance
  parameter: Authorization
  sources:
  - developer.frontify.com
  - help.frontify.com
  type: apiKey
- authorizationUrl: https://mcp.frontify-integrations.com/oauth/authorize
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  description: 'The MCP server runs its own authorization server implementing the MCP 2025-11-25 authorization spec — RFC 8414 AS metadata, RFC 9728 protected-resource metadata, PKCE S256, public clients (token_endpoint_auth_method none), and BOTH client registration approaches: Client ID Metadata Documents and Dynamic Client Registration. A user authorizes access to their Frontify instance on first connection; the server then brokers to the instance under the pack''s Frontify scopes.'
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.frontify-integrations.com
  name: OAuth2 (Authorization Code + PKCE) — MCP authorization server
  protected_resource: https://mcp.frontify-integrations.com/mcp
  registrationUrl: https://mcp.frontify-integrations.com/oauth/register
  response_types_supported:
  - code
  scopes_supported:
  - mcp:tools
  - openid
  sources:
  - well-known/frontify-oauth-authorization-server.json
  - well-known/frontify-oauth-protected-resource.json
  - well-known/frontify-openid-configuration.json
  tokenUrl: https://mcp.frontify-integrations.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: frontify-authentication
source_filename: frontify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  well-known/frontify-oauth-authorization-server.json +\n  well-known/frontify-oauth-protected-resource.json (both fetched live from the Frontify\n  MCP host) + the WWW-Authenticate challenge observed on an anonymous MCP tools/list POST\n  + live GraphQL permission-error probes + Frontify's own MCP pack pages +\n  https://developer.frontify.com/ and npm @frontify/frontify-authenticator\ndocs: https://help.frontify.com/en/articles/5402357-getting-started-with-the-frontify-graphql-api\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: S256 (MCP authorization server)\n  dynamic_client_registration: true (MCP authorization server, RFC 7591)\n  note: >-\n    Frontify publishes no OpenAPI, so this profile is not derived from securitySchemes.\n    It is assembled from two RFC-compliant discovery documents Frontify actually serves,\n    the live 401 challenge on its MCP endpoint,\
  \ and observed GraphQL permission errors.\nsurfaces:\n  - name: Frontify GraphQL API\n    endpoint: https://{instance}.frontify.com/graphql\n    schemes: [OAuth2 (Authorization Code), API Token (Bearer)]\n    anonymous_behavior: >-\n      Schema introspection succeeds anonymously (HTTP 200, full schema). Any data field\n      returns HTTP 200 with errors[0].message \"UserId not set in identity.\" or\n      \"policy 'authenticated' not fulfilled\" and extensions.category \"permission\".\n      Introspection is open; data is not.\n  - name: Frontify MCP Server\n    endpoint: https://mcp.frontify-integrations.com/mcp\n    schemes: [OAuth2 (Authorization Code + PKCE)]\n    anonymous_behavior: >-\n      HTTP 401 with a spec-conformant challenge:\n      WWW-Authenticate: Bearer resource_metadata=\"…/.well-known/oauth-protected-resource/mcp\",\n      scope=\"mcp:tools\"\nschemes:\n  - name: OAuth2 (Authorization Code) — Frontify instance\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl:\
  \ https://{instance}.frontify.com/api/oauth/authorize\n    description: >-\n      Interactive OAuth 2.0 authorization against a user's Frontify instance — used by\n      the Frontify Authenticator, Finder, Brand SDK apps and custom integrations. Client\n      ID / Client Secret are issued by creating an OAuth application in the instance's\n      Developer settings; the scope set requested at registration must match the scope\n      set requested at authorization.\n    scopes: scopes/frontify-scopes.yml\n    sources: [developer.frontify.com, \"@frontify/frontify-authenticator\", third-party connector docs]\n  - name: API Token (Bearer) — Frontify instance\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: Bearer <token>\n    description: >-\n      Personal / API access tokens generated per Frontify instance, sent as a Bearer\n      token for server-to-server GraphQL calls. Frontify's knowledge base notes API\n      access must be enabled on the account.\n    sources:\
  \ [developer.frontify.com, help.frontify.com]\n  - name: OAuth2 (Authorization Code + PKCE) — MCP authorization server\n    type: oauth2\n    flow: authorizationCode\n    issuer: https://mcp.frontify-integrations.com\n    authorizationUrl: https://mcp.frontify-integrations.com/oauth/authorize\n    tokenUrl: https://mcp.frontify-integrations.com/oauth/token\n    registrationUrl: https://mcp.frontify-integrations.com/oauth/register\n    scopes_supported: [mcp:tools, openid]\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none]\n    client_id_metadata_document_supported: true\n    bearer_methods_supported: [header]\n    protected_resource: https://mcp.frontify-integrations.com/mcp\n    description: >-\n      The MCP server runs its own authorization server implementing the MCP 2025-11-25\n      authorization spec — RFC 8414 AS metadata, RFC 9728\
  \ protected-resource metadata,\n      PKCE S256, public clients (token_endpoint_auth_method none), and BOTH client\n      registration approaches: Client ID Metadata Documents and Dynamic Client\n      Registration. A user authorizes access to their Frontify instance on first\n      connection; the server then brokers to the instance under the pack's Frontify\n      scopes.\n    sources:\n      - well-known/frontify-oauth-authorization-server.json\n      - well-known/frontify-oauth-protected-resource.json\n      - well-known/frontify-openid-configuration.json\nsso:\n  note: >-\n    Frontify supports SAML SSO for platform users (Microsoft Entra / Azure AD documented\n    examples, SSO user-group mapping). That is end-user authentication to the product,\n    not API authentication, and is out of scope for this profile.\n  source: help.frontify.com SSO articles\nprobes:\n  - url: https://mcp.frontify-integrations.com/.well-known/oauth-authorization-server\n    http_status: 200\n    checked:\
  \ '2026-08-13'\n  - url: https://mcp.frontify-integrations.com/.well-known/oauth-protected-resource\n    http_status: 200\n    checked: '2026-08-13'\n  - url: https://mcp.frontify-integrations.com/mcp\n    http_status: 401\n    result: OAuth challenge, scope=\"mcp:tools\"\n    checked: '2026-08-13'\n  - url: https://api.frontify.com/graphql\n    http_status: 200\n    result: 'anonymous data query -> extensions.category \"permission\"'\n    checked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontify/refs/heads/main/authentication/frontify-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Company
- Marketing
- Brand Management
- Digital Asset Management
- DAM
- Content
- GraphQL
- Creative Operations
---
