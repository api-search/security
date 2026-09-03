---
api_key_in: []
auth_types: []
description: 'Verto Education exposes exactly one authenticated machine surface: the remote MCP endpoint at https://vertoeducation.org/wp-json/mcp/mcp-oauth-server, fronted by an OAuth 2.0 authorization server on the same origin. This profile is read directly from the two live discovery documents (RFC 8414 and RFC 9728), not from an OpenAPI securityScheme - Verto publishes no OpenAPI. There is no public developer portal, no API key programme, and no documented auth page; everything recorded here was established by probe.'
kind: authentication
layout: security
method: probed
name: Verto Education Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verto Education declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Verto Education
provider_slug: verto-education
scheme_count: 2
schemes:
- applies_to:
  - https://vertoeducation.org/wp-json/mcp/mcp-oauth-server
  bearer_format: Bearer
  client_authentication:
  - none
  client_authentication_note: token_endpoint_auth_methods_supported is ["none"], i.e. public clients only. There is no client_secret_basic or client_secret_post, and no RFC 7591 dynamic client registration endpoint is advertised; the server sets client_id_metadata_document_supported true instead, so a client is identified by a URL pointing at its own metadata document.
  flows:
    authorization_code:
      authorization_url: https://vertoeducation.org/oauth/authorize
      pkce_methods:
      - S256
      pkce_required: true
      refresh_url: https://vertoeducation.org/oauth/token
      revocation_url: https://vertoeducation.org/oauth/revoke
      scopes:
        mcp: The only scope the authorization server advertises. Its exact grant surface is not documented by the provider; it gates the MCP endpoint named in the protected-resource metadata.
      token_url: https://vertoeducation.org/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2
  in: header
  response_types:
  - code
  scheme: OAuth 2.0 authorization code with PKCE
  type: oauth2
- applies_to:
  - https://vertoeducation.org/wp-json/
  id: wordpress-rest-session
  note: The entire WordPress REST API on this host is closed to anonymous callers. /wp-json, /wp-json/wp/v2, /wp-json/wp/v2/posts and /?rest_route=/ each return HTTP 401 {"code":"rest_not_logged_in"}. This is a deliberate hardening choice, not a misconfiguration, and it means no anonymous content API exists here.
  scheme: cookie/session (WordPress)
  type: http
slug: verto-education-authentication
source_filename: verto-education-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://vertoeducation.org/.well-known/oauth-authorization-server\nname: Verto Education Authentication\ndescription: >-\n  Verto Education exposes exactly one authenticated machine surface: the remote MCP\n  endpoint at https://vertoeducation.org/wp-json/mcp/mcp-oauth-server, fronted by an\n  OAuth 2.0 authorization server on the same origin. This profile is read directly\n  from the two live discovery documents (RFC 8414 and RFC 9728), not from an OpenAPI\n  securityScheme - Verto publishes no OpenAPI. There is no public developer portal,\n  no API key programme, and no documented auth page; everything recorded here was\n  established by probe.\nschemes:\n- id: oauth2\n  type: oauth2\n  scheme: OAuth 2.0 authorization code with PKCE\n  in: header\n  bearer_format: Bearer\n  flows:\n    authorization_code:\n      authorization_url: https://vertoeducation.org/oauth/authorize\n      token_url: https://vertoeducation.org/oauth/token\n\
  \      revocation_url: https://vertoeducation.org/oauth/revoke\n      refresh_url: https://vertoeducation.org/oauth/token\n      pkce_required: true\n      pkce_methods:\n      - S256\n      scopes:\n        mcp: >-\n          The only scope the authorization server advertises. Its exact grant surface\n          is not documented by the provider; it gates the MCP endpoint named in the\n          protected-resource metadata.\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  client_authentication:\n  - none\n  client_authentication_note: >-\n    token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients only. There\n    is no client_secret_basic or client_secret_post, and no RFC 7591 dynamic client\n    registration endpoint is advertised; the server sets\n    client_id_metadata_document_supported true instead, so a client is identified by a\n    URL pointing at its own metadata document.\n  applies_to:\n  - https://vertoeducation.org/wp-json/mcp/mcp-oauth-server\n\
  - id: wordpress-rest-session\n  type: http\n  scheme: cookie/session (WordPress)\n  applies_to:\n  - https://vertoeducation.org/wp-json/\n  note: >-\n    The entire WordPress REST API on this host is closed to anonymous callers. /wp-json,\n    /wp-json/wp/v2, /wp-json/wp/v2/posts and /?rest_route=/ each return HTTP 401\n    {\"code\":\"rest_not_logged_in\"}. This is a deliberate hardening choice, not a\n    misconfiguration, and it means no anonymous content API exists here.\nopenid_connect: false\nopenid_connect_note: >-\n  /.well-known/openid-configuration returns the WordPress 404 template. The server is\n  a bare OAuth 2.0 authorization server, not an OIDC provider - no id_token, no userinfo\n  endpoint, no jwks_uri advertised.\nmtls: false\napi_keys: false\ndocs: null\ndocs_note: >-\n  Verto publishes no authentication documentation. The auth surface is discoverable only\n  from the machine-readable metadata documents, which is unusually good machine\n  discoverability paired with\
  \ zero human documentation.\nx-evidence:\n- url: https://vertoeducation.org/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://vertoeducation.org/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://vertoeducation.org/.well-known/openid-configuration\n  http_status: 404\n- url: https://vertoeducation.org/wp-json/\n  http_status: 401\n- url: https://vertoeducation.org/oauth/token\n  http_status: 405\nchecked: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verto-education/refs/heads/main/authentication/verto-education-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Education
- Higher Education
- Study Abroad
- College Admissions
- Students
- Travel
- Model Context Protocol
- OAuth
- Agents
---
