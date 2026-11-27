---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clonio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clonio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clonio
provider_slug: clonio-es
scheme_count: 1
schemes:
- applies_to: https://clonio.es/api/mcp
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  dynamic_client_registration: https://clonio.es/api/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://clonio.es/oauth/authorize
      refreshUrl: https://clonio.es/api/oauth/token
      tokenUrl: https://clonio.es/api/oauth/token
  name: oauth2
  pkce: S256
  revocation_endpoint: https://clonio.es/api/oauth/revoke
  scopes:
  - account:read
  - posts:read
  - posts:write
  - posts:publish
  - insights:read
  - ai:generate
  - images:generate
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: clonio-es-authentication
source_filename: clonio-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clonio.es/.well-known/oauth-authorization-server\ndocs: https://clonio.es/ayuda/mcp\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://clonio.es/api/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clonio.es/oauth/authorize\n      tokenUrl: https://clonio.es/api/oauth/token\n      refreshUrl: https://clonio.es/api/oauth/token\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  dynamic_client_registration: https://clonio.es/api/oauth/register\n  client_id_metadata_document_supported: true\n  revocation_endpoint: https://clonio.es/api/oauth/revoke\n  bearer_methods: [header]\n  scopes: [account:read, posts:read, posts:write, posts:publish, insights:read, ai:generate, images:generate]\ndiscovery:\n  protected_resource_metadata: {url: https://clonio.es/.well-known/oauth-protected-resource, http_status: 200}\n  authorization_server_metadata: {url: https://clonio.es/.well-known/oauth-authorization-server,\
  \ http_status: 200}\nnote: Values read from the two published RFC 9728 / RFC 8414 discovery documents (GET only; no auth endpoint was called). The docs say the user picks permissions on the consent screen, sensitive ones (publish to LinkedIn, spending image credits outside Claude) are pre-checked but can be unchecked, and connections are revoked under Configuración → Conexiones.\n"
source_yaml_url: https://artifacts.apis.io/clonio-es/authentication/clonio-es-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LinkedIn
- Content Generation
- Social Media
- Marketing
- Scheduling
- MCP
---
