---
api_key_in:
- header
api_specs:
- filename: endeavor-biomedicines-wordpress-rest-openapi.yml
  format: yaml
  label: Endeavor BioMedicines WordPress REST API
  slug: endeavor-biomedicines-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wordpress-rest-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Endeavor Biomedicines Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Endeavor BioMedicines secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Endeavor BioMedicines
provider_slug: endeavor-biomedicines
scheme_count: 3
schemes:
- description: WordPress cookie-authenticated nonce. Advertised by the host in Access-Control-Allow-Headers on every /wp-json response.
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/endeavor-biomedicines-wordpress-rest-openapi.yml
  type: apiKey
- description: Bearer token in the Authorization header, advertised by the host in Access-Control-Allow-Headers.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/endeavor-biomedicines-wordpress-rest-openapi.yml
  type: http
- description: OAuth 2.1 authorization-code flow with PKCE (S256) protecting the MCP endpoint. token_endpoint_auth_methods_supported is ["none"] — public clients — and client_id_metadata_document_supported is true, so clients identify themselves with a client-ID metadata document rather than a registration endpoint.
  flows:
    authorizationCode:
      authorizationUrl: https://endeavorbiomedicines.com/oauth/authorize
      refreshUrl: https://endeavorbiomedicines.com/oauth/token
      scopes:
        mcp: Access the WordPress MCP server on this host.
      tokenUrl: https://endeavorbiomedicines.com/oauth/token
  name: mcpOAuth
  sources:
  - well-known/endeavor-biomedicines-oauth-authorization-server.json
  - well-known/endeavor-biomedicines-oauth-protected-resource.json
  type: oauth2
slug: endeavor-biomedicines-authentication
source_filename: endeavor-biomedicines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  openapi/endeavor-biomedicines-wordpress-rest-openapi.yml +\n  https://endeavorbiomedicines.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  There is no published authentication documentation. The profile below is derived\n  from the OpenAPI this pipeline built from the host's own /wp-json/ route index and\n  upgraded with the OAuth 2.1 metadata the host serves anonymously.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  anonymous_read: true\n  anonymous_read_note: >-\n    Content reads (/wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories,\n    /wp/v2/types) return HTTP 200 with no credentials — verified live on 2026-08-12.\n    Write and administrative operations return 401/403.\nschemes:\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: >-\n    WordPress cookie-authenticated\
  \ nonce. Advertised by the host in\n    Access-Control-Allow-Headers on every /wp-json response.\n  sources:\n  - openapi/endeavor-biomedicines-wordpress-rest-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token in the Authorization header, advertised by the host in\n    Access-Control-Allow-Headers.\n  sources:\n  - openapi/endeavor-biomedicines-wordpress-rest-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE (S256) protecting the MCP endpoint.\n    token_endpoint_auth_methods_supported is [\"none\"] — public clients — and\n    client_id_metadata_document_supported is true, so clients identify themselves\n    with a client-ID metadata document rather than a registration endpoint.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://endeavorbiomedicines.com/oauth/authorize\n      tokenUrl: https://endeavorbiomedicines.com/oauth/token\n      refreshUrl: https://endeavorbiomedicines.com/oauth/token\n\
  \      scopes:\n        mcp: Access the WordPress MCP server on this host.\n  sources:\n  - well-known/endeavor-biomedicines-oauth-authorization-server.json\n  - well-known/endeavor-biomedicines-oauth-protected-resource.json\nx-evidence:\n- fetched: '2026-08-12'\n  url: https://endeavorbiomedicines.com/wp-json/wp/v2/posts?per_page=1\n  http_status: 200\n  note: anonymous read succeeds\n- fetched: '2026-08-12'\n  url: https://endeavorbiomedicines.com/wp-json/mcp/mcp-oauth-server\n  http_status: 401\n  note: MCP requires an OAuth 2.1 bearer token in the \"mcp\" scope\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/authentication/endeavor-biomedicines-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Healthcare
- Drug Development
- Content
- WordPress
---
