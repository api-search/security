---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Docsend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: DocSend secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: DocSend
provider_slug: docsend
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://docsend.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://docsend.com/oauth/token
    scopes:
      analytics:read: Read access to viewer/page engagement analytics
      contacts:read: Read access to contacts / visitors
      documents:read: Read access to DocSend documents and share links
      spaces:read: Read access to DocSend Spaces (virtual data rooms)
      spaces:write: Write access to DocSend Spaces (virtual data rooms)
    tokenUrl: https://docsend.com/oauth/token
  - flow: clientCredentials
    scopes:
      analytics:read: Read access to viewer/page engagement analytics
      contacts:read: Read access to contacts / visitors
      documents:read: Read access to DocSend documents and share links
      spaces:read: Read access to DocSend Spaces (virtual data rooms)
      spaces:write: Write access to DocSend Spaces (virtual data rooms)
    tokenUrl: https://docsend.com/oauth/token
  name: OAuth2
  registration_endpoint: https://docsend.com/oauth/register
  revocation_endpoint: https://docsend.com/oauth/revoke
  sources:
  - well-known/docsend-oauth-authorization-server.json
  - well-known/docsend-mcp-host-oauth-authorization-server.json
  - well-known/docsend-oauth-protected-resource-mcp.json
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: docsend-authentication
source_filename: docsend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://docsend.com/.well-known/oauth-authorization-server (RFC 8414),\n  https://mcp.docsend.com/.well-known/oauth-authorization-server (RFC 8414),\n  https://docsend.com/.well-known/oauth-protected-resource/mcp (RFC 9728), and the\n  WWW-Authenticate challenge returned by https://docsend.com/mcp and\n  https://mcp.docsend.com/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]\n  bearer_methods: [header]\n  protected_resource_metadata: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n  - well-known/docsend-mcp-host-oauth-authorization-server.json\n  - well-known/docsend-oauth-protected-resource-mcp.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docsend.com/oauth/authorize\n    tokenUrl:\
  \ https://docsend.com/oauth/token\n    refreshUrl: https://docsend.com/oauth/token\n    scopes:\n      documents:read: Read access to DocSend documents and share links\n      spaces:read: Read access to DocSend Spaces (virtual data rooms)\n      spaces:write: Write access to DocSend Spaces (virtual data rooms)\n      analytics:read: Read access to viewer/page engagement analytics\n      contacts:read: Read access to contacts / visitors\n  - flow: clientCredentials\n    tokenUrl: https://docsend.com/oauth/token\n    scopes:\n      documents:read: Read access to DocSend documents and share links\n      spaces:read: Read access to DocSend Spaces (virtual data rooms)\n      spaces:write: Write access to DocSend Spaces (virtual data rooms)\n      analytics:read: Read access to viewer/page engagement analytics\n      contacts:read: Read access to contacts / visitors\n  registration_endpoint: https://docsend.com/oauth/register\n  revocation_endpoint: https://docsend.com/oauth/revoke\n  code_challenge_methods:\
  \ [S256]\n  token_endpoint_auth_methods: [none]\nissuers:\n- issuer: https://docsend.com\n  metadata: https://docsend.com/.well-known/oauth-authorization-server\n- issuer: https://mcp.docsend.com\n  metadata: https://mcp.docsend.com/.well-known/oauth-authorization-server\n  note: >-\n    Advertises the same endpoints on docsend.com; the RFC 9728 resource document names\n    https://docsend.com as the sole authorization server.\nprotected_resource:\n  resource: https://docsend.com/mcp\n  metadata: https://docsend.com/.well-known/oauth-protected-resource/mcp\n  authorization_servers: [https://docsend.com]\n  bearer_methods_supported: [header]\ndocs: null\nnotes: >-\n  DocSend operates a full OAuth 2.0 authorization server with RFC 8414 discovery, RFC 7591\n  dynamic client registration, RFC 7636 PKCE (S256 mandatory), RFC 7009 token revocation\n  and RFC 9728 protected-resource metadata. token_endpoint_auth_methods_supported is\n  [\"none\"], i.e. public clients registering dynamically and\
  \ authenticating with PKCE —\n  the standard MCP client shape. This authorization surface exists to gate the hosted MCP\n  server; DocSend publishes no general-purpose REST API and no OpenAPI, and no readable\n  authentication documentation page (www.docsend.com and help.docsend.com return HTTP 403\n  to non-browser clients), so this profile is built entirely from the machine-readable\n  discovery documents DocSend serves.\nchanges_since_last_round:\n  checked: '2026-08-14'\n  previous: '2026-07-18'\n  notes: >-\n    Scopes changed from mcp:read / mcp:write to five resource-scoped values, and RFC 9728\n    protected-resource metadata appeared (it 404d on the previous pass).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsend/refs/heads/main/authentication/docsend-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Document Sharing
- Sales Enablement
- Analytics
- Data Room
- E-Signature
- MCP
- Dropbox
---
