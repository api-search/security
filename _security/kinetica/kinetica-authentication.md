---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kinetica Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kinetica secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kinetica
provider_slug: kinetica
scheme_count: 4
schemes:
- description: Database username and password sent as HTTP Basic credentials on every POST. All Kinetica REST endpoints require POST.
  example_header: 'Authorization: Basic <base64(user:pass)>'
  in: header
  name: basicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - https://docs.kinetica.com/content/api/concepts
  - https://github.com/kineticadb/agent-skills/blob/main/knowledge/curl-api-reference.md
  surface: Kinetica Database REST API
  type: http
- description: OAuth 2.0 bearer token, documented as the preferred mechanism when the deployment has SSO configured. Kinetica 7.2.2 added single sign-on across its UI platforms.
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://github.com/kineticadb/agent-skills/blob/main/knowledge/curl-api-reference.md
  surface: Kinetica Database REST API
  type: http
- authorization_server_metadata: https://app.toolbelt.ai/.well-known/oauth-authorization-server
  bearer_methods:
  - header
  flows:
  - authorizationUrl: https://app.toolbelt.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://app.toolbelt.ai/oauth/register
    scopes:
      mcp:tools: Invoke the toolbelt_* MCP tools against the connected Kinetica database
      openid: OpenID Connect subject identity
    tokenUrl: https://app.toolbelt.ai/oauth/token
  name: toolbeltOAuth2
  protected_resource_metadata: https://mcp.toolbelt.ai/.well-known/oauth-protected-resource
  refresh_supported: true
  sources:
  - well-known/kinetica-toolbelt-oauth-protected-resource.json
  - well-known/kinetica-toolbelt-oauth-authorization-server.json
  standards:
  - RFC 6749
  - RFC 7636
  - RFC 7591
  - RFC 8414
  - RFC 9728
  surface: Kinetica Toolbelt MCP Server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- description: The documentation MCP server declares authentication:none in its published manifest and answers tools/list anonymously.
  name: none
  sources:
  - https://docs.kinetica.com/.well-known/mcp.json
  surface: Kinetica Docs MCP Server
  type: none
slug: kinetica-authentication
source_filename: kinetica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.kinetica.com/content/api/concepts and https://github.com/kineticadb/agent-skills/blob/main/knowledge/curl-api-reference.md\ndocs: https://docs.kinetica.com/7.2/api/\nnote: Kinetica publishes no OpenAPI document, so this profile is read from the published\n  API concepts / REST access documentation rather than derived from securitySchemes.\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  surfaces:\n  - Kinetica Database REST API\n  - Kinetica Toolbelt MCP Server\n  - Kinetica Docs MCP Server\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  surface: Kinetica Database REST API\n  in: header\n  parameter: Authorization\n  description: Database username and password sent as HTTP Basic credentials on every\n    POST. All Kinetica REST endpoints require POST.\n  example_header: 'Authorization: Basic <base64(user:pass)>'\n  sources:\n  - https://docs.kinetica.com/content/api/concepts\n\
  \  - https://github.com/kineticadb/agent-skills/blob/main/knowledge/curl-api-reference.md\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: Kinetica Database REST API\n  in: header\n  parameter: Authorization\n  description: OAuth 2.0 bearer token, documented as the preferred mechanism when the\n    deployment has SSO configured. Kinetica 7.2.2 added single sign-on across its UI\n    platforms.\n  sources:\n  - https://github.com/kineticadb/agent-skills/blob/main/knowledge/curl-api-reference.md\n- name: toolbeltOAuth2\n  type: oauth2\n  surface: Kinetica Toolbelt MCP Server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.toolbelt.ai/oauth/authorize\n    tokenUrl: https://app.toolbelt.ai/oauth/token\n    registrationUrl: https://app.toolbelt.ai/oauth/register\n    pkce: S256\n    scopes:\n      mcp:tools: Invoke the toolbelt_* MCP tools against the connected Kinetica database\n      openid: OpenID Connect subject identity\n  refresh_supported: true\n\
  \  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  bearer_methods:\n  - header\n  protected_resource_metadata: https://mcp.toolbelt.ai/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://app.toolbelt.ai/.well-known/oauth-authorization-server\n  standards:\n  - RFC 6749\n  - RFC 7636\n  - RFC 7591\n  - RFC 8414\n  - RFC 9728\n  sources:\n  - well-known/kinetica-toolbelt-oauth-protected-resource.json\n  - well-known/kinetica-toolbelt-oauth-authorization-server.json\n- name: none\n  type: none\n  surface: Kinetica Docs MCP Server\n  description: The documentation MCP server declares authentication:none in its published\n    manifest and answers tools/list anonymously.\n  sources:\n  - https://docs.kinetica.com/.well-known/mcp.json\nin_database_authorization:\n  model: PostgreSQL-style GRANT/REVOKE with Kinetica extensions\n  external_identity: LDAP users are created with an @ prefix (CREATE USER \"@ldap_user\")\n  system_permissions:\n  - SYSTEM\
  \ ADMIN\n  - SYSTEM CREATE\n  - SYSTEM MONITOR\n  - SYSTEM READ\n  - SYSTEM WRITE\n  - USER ADMIN\n  object_permissions:\n  - schema-level (ALL, SELECT, CREATE TABLE, INSERT, UPDATE, DELETE)\n  - table-level (SELECT, INSERT, UPDATE, ALL, WITH GRANT OPTION)\n  extras:\n  - row-level security\n  - column masking\n  - resource groups\n  introspection: SHOW SECURITY FOR \"<user-or-role>\"\n  source: https://github.com/kineticadb/agent-skills/blob/main/knowledge/security-reference.md\ntransport_security:\n  https_supported: true\n  note: Kinetica deployments commonly present self-signed certificates; client libraries\n    expose an explicit certificate-verification bypass (setBypassSslCertCheck / skip_ssl_cert_verification,\n    default false) and the documented curl examples use -k.\n  source: https://docs.kinetica.com/content/api/concepts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinetica/refs/heads/main/authentication/kinetica-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Database
- Analytics
- gpu-acceleration
- Real-Time Analytics
- Vector Search
- Graph Analytics
- Geospatial
- Time Series
- SQL
- Streaming
- Data Infrastructure
- MCP
- agent-native
- RAG
---
