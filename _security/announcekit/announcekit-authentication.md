---
api_key_in: []
auth_types: []
description: 'AnnounceKit has no OpenAPI securitySchemes to derive from - the contract is GraphQL - so this profile is assembled from the documented auth paths and the live OAuth metadata. Four distinct schemes coexist: Basic auth on the GraphQL endpoint, ak_pat_ bearer tokens for the MCP server, a full OAuth 2.0 authorization-code + PKCE flow behind the hosted MCP login, and JWT-signed user identity for the client-side widget.'
kind: authentication
layout: security
method: searched
name: Announcekit Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnnounceKit declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: AnnounceKit
provider_slug: announcekit
scheme_count: 4
schemes:
- description: 'The documented way to call the GraphQL API directly: a Basic Authentication token supplied in the request header. AnnounceKit''s docs also accept the dashboard login cookies (sesid, sesid.sig) for browser-side use, and the GraphiQL IDE works with no explicit credential once signed in.'
  documented: https://announcekit.app/docs/graphql-api
  header: Authorization
  id: graphql-basic
  in: header
  scheme: basic
  surface: https://announcekit.app/gq/v2
  type: http
- description: Project-scoped access tokens created under Settings > API Tokens (owners and managers only). Shown once at creation. Two scopes, read and write. A token acts on behalf of the member who created it and inherits that member's role and project access; if the member loses access, the token stops working.
  documented: https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit
  header: Authorization
  id: personal-access-token
  in: header
  schema_backing:
    fields:
    - id
    - name
    - prefix
    - scope
    - created_by
    - created_at
    - last_used_at
    - expires_at
    note: The schema carries expires_at and last_used_at, so tokens are expirable and their use is tracked, though the docs do not state a default lifetime.
    type: AccessToken
  scheme: bearer
  surface: https://mcp.announcekit.app/mcp
  token_prefix: ak_pat_
  type: http
- authorization_endpoint: https://announcekit.app/oauth/authorize
  description: The hosted MCP login flow. An MCP client discovers the authorization server from the protected-resource metadata, registers itself dynamically, and sends the user to AnnounceKit to log in and approve - no token is copied by hand. Grants are listed and revocable under Settings > Connected apps, with a ceiling of 10 connected apps per user.
  dynamic_client_registration: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2
  issuer: https://announcekit.app
  pkce: S256
  probed:
    fetched: '2026-09-02'
    file: well-known/announcekit-oauth-authorization-server.json
    http_status: 200
    url: https://announcekit.app/.well-known/oauth-authorization-server
  registration_endpoint: https://announcekit.app/oauth/register
  response_types:
  - code
  schema_backing:
    fields:
    - id
    - client_name
    - scope
    - created_at
    - last_used_at
    type: ConnectedApp
  scopes:
    read: View posts, feedback, stats and roadmap.
    write: Read, plus create and update content. No deletes.
  surface: https://mcp.announcekit.app/mcp
  token_endpoint: https://announcekit.app/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- description: Signed user tracking. The host application signs the end user's identity as a JSON Web Token so the widget can verify who it is showing targeted or private content to, preventing client-side spoofing of user attributes. This authenticates the END USER to the widget, not a developer to the API.
  documented: https://announcekit.app/docs/json-web-tokens
  id: widget-jwt
  in: client
  surface: In-app widget / user tracking
  type: jwt
slug: announcekit-authentication
source_filename: announcekit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://announcekit.app/docs/graphql-api,\n  https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit,\n  https://help.announcekit.app/en/articles/6583616-jwt-user-authentication,\n  https://announcekit.app/security, the probed RFC 8414 metadata at\n  https://announcekit.app/.well-known/oauth-authorization-server (HTTP 200) and\n  RFC 9728 metadata at\n  https://mcp.announcekit.app/.well-known/oauth-protected-resource (HTTP 200),\n  and the introspected GraphQL schema (AccessToken, ConnectedApp, SAMLConfig,\n  TOTPConfig types), 2026-09-02.\nprovider: AnnounceKit\nproviderId: announcekit\ndescription: >-\n  AnnounceKit has no OpenAPI securitySchemes to derive from - the contract is\n  GraphQL - so this profile is assembled from the documented auth paths and the\n  live OAuth metadata. Four distinct schemes coexist: Basic auth on the GraphQL\n  endpoint, ak_pat_ bearer tokens\
  \ for the MCP server, a full OAuth 2.0\n  authorization-code + PKCE flow behind the hosted MCP login, and JWT-signed\n  user identity for the client-side widget.\nschemes:\n- id: graphql-basic\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  surface: https://announcekit.app/gq/v2\n  description: >-\n    The documented way to call the GraphQL API directly: a Basic Authentication\n    token supplied in the request header. AnnounceKit's docs also accept the\n    dashboard login cookies (sesid, sesid.sig) for browser-side use, and the\n    GraphiQL IDE works with no explicit credential once signed in.\n  documented: https://announcekit.app/docs/graphql-api\n- id: personal-access-token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  token_prefix: ak_pat_\n  surface: https://mcp.announcekit.app/mcp\n  description: >-\n    Project-scoped access tokens created under Settings > API Tokens (owners and\n    managers only). Shown once at creation.\
  \ Two scopes, read and write. A token\n    acts on behalf of the member who created it and inherits that member's role\n    and project access; if the member loses access, the token stops working.\n  schema_backing:\n    type: AccessToken\n    fields: [id, name, prefix, scope, created_by, created_at, last_used_at, expires_at]\n    note: >-\n      The schema carries expires_at and last_used_at, so tokens are expirable and\n      their use is tracked, though the docs do not state a default lifetime.\n  documented: https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  dynamic_client_registration: true\n  issuer: https://announcekit.app\n  authorization_endpoint: https://announcekit.app/oauth/authorize\n  token_endpoint: https://announcekit.app/oauth/token\n  registration_endpoint: https://announcekit.app/oauth/register\n  grant_types: [authorization_code, refresh_token]\n\
  \  response_types: [code]\n  token_endpoint_auth_methods: [none]\n  scopes:\n    read: View posts, feedback, stats and roadmap.\n    write: Read, plus create and update content. No deletes.\n  surface: https://mcp.announcekit.app/mcp\n  description: >-\n    The hosted MCP login flow. An MCP client discovers the authorization server\n    from the protected-resource metadata, registers itself dynamically, and\n    sends the user to AnnounceKit to log in and approve - no token is copied by\n    hand. Grants are listed and revocable under Settings > Connected apps, with\n    a ceiling of 10 connected apps per user.\n  schema_backing:\n    type: ConnectedApp\n    fields: [id, client_name, scope, created_at, last_used_at]\n  probed:\n    url: https://announcekit.app/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-09-02'\n    file: well-known/announcekit-oauth-authorization-server.json\n- id: widget-jwt\n  type: jwt\n  in: client\n  surface: In-app widget / user\
  \ tracking\n  description: >-\n    Signed user tracking. The host application signs the end user's identity as\n    a JSON Web Token so the widget can verify who it is showing targeted or\n    private content to, preventing client-side spoofing of user attributes.\n    This authenticates the END USER to the widget, not a developer to the API.\n  documented: https://announcekit.app/docs/json-web-tokens\ndashboard_authentication:\n- name: SAML 2.0 Single Sign-On\n  availability: Scale and Enterprise plans\n  schema_backing: {type: SAMLConfig, query: samlConfig, login: samlLoginURL}\n  documented: https://announcekit.app/security\n- name: TOTP two-factor authentication\n  availability: All plans, all team members\n  schema_backing: {type: TOTPConfig, mutations: [createTotpConfig, activateTotpConfig, removeTotpConfig]}\n- name: Role-based access control\n  roles: [owner, manager, editor, viewer]\n  schema_backing: {enum: ProjectRole}\n  note: >-\n    The four roles are declared in the live\
  \ GraphQL schema as the ProjectRole\n    enum, which matches the four roles named on the security page.\n- name: IP access control\n  availability: Enterprise plans\n  documented: https://announcekit.app/security\ngaps:\n- >-\n  The Basic Authentication scheme on the GraphQL endpoint is documented without\n  naming the header format or what the two halves of the credential are; the\n  docs say \"supply a Basic Authentication token in request Header\" and stop\n  there. An implementer has to infer it.\n- >-\n  No documented token rotation or expiry policy for ak_pat_ tokens, even though\n  the schema exposes an expires_at field.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/announcekit/refs/heads/main/authentication/announcekit-authentication.yml
summary_line: 4 schemes
tags:
- Changelog
- Feature Requests
- NPS
- Notification
- Product Communication
- Roadmaps
- Software-as-a-Service
- Widgets
---
