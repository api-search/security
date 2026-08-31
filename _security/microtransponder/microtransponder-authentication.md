---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Microtransponder Authentication
name_suffix: Authentication
oauth_flows: []
overview: MicroTransponder declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MicroTransponder
provider_slug: microtransponder
scheme_count: 3
schemes:
- applies_to: GET on the public wp/v2 collections (posts, pages, media, news, team, categories, tags, search, types, taxonomies) and the REST root at /wp-json/
  evidence: GET https://www.mobia.com/wp-json/wp/v2/news?per_page=2 -> 200
  id: anonymous_read
  type: none
- applies_to: https://www.mobia.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://www.mobia.com/oauth/authorize
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  evidence: https://www.mobia.com/.well-known/oauth-authorization-server -> 200
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2
  issuer: https://www.mobia.com
  pkce: S256
  response_types_supported:
  - code
  revocation_endpoint: https://www.mobia.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://www.mobia.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: All wp/v2 write operations, /wp-abilities/v1/.../run, and /wp-json/mcp/mcp-adapter-default-server
  evidence: POST https://www.mobia.com/wp-json/mcp/mcp-adapter-default-server -> 401 {"code":"rest_forbidden"}
  id: wordpress_credentialed
  note: WordPress core authentication (login cookie + X-WP-Nonce, or an Application Password over HTTP Basic). Not documented by the provider; inferred from the standard WordPress error contract returned by this host.
  scheme: cookie-or-application-password
  type: http
slug: microtransponder-authentication
source_filename: microtransponder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://www.mobia.com/.well-known/oauth-authorization-server +\n  https://www.mobia.com/.well-known/oauth-protected-resource + observed 401 responses on\n  https://www.mobia.com/wp-json/\nnote: >-\n  Derived entirely from documents the host actually served and responses actually\n  observed. The company publishes no authentication documentation of its own — there is\n  no developer portal — so nothing here comes from prose.\napi: Mobia Medical Site REST API (WordPress)\nschemes:\n- id: anonymous_read\n  type: none\n  applies_to: >-\n    GET on the public wp/v2 collections (posts, pages, media, news, team, categories,\n    tags, search, types, taxonomies) and the REST root at /wp-json/\n  evidence: GET https://www.mobia.com/wp-json/wp/v2/news?per_page=2 -> 200\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  applies_to: https://www.mobia.com/wp-json/mcp/mcp-oauth-server\n  issuer: https://www.mobia.com\n\
  \  authorization_endpoint: https://www.mobia.com/oauth/authorize\n  token_endpoint: https://www.mobia.com/oauth/token\n  revocation_endpoint: https://www.mobia.com/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  client_id_metadata_document_supported: true\n  bearer_methods_supported:\n  - header\n  scopes:\n  - mcp\n  evidence: https://www.mobia.com/.well-known/oauth-authorization-server -> 200\n- id: wordpress_credentialed\n  type: http\n  scheme: cookie-or-application-password\n  applies_to: >-\n    All wp/v2 write operations, /wp-abilities/v1/.../run, and\n    /wp-json/mcp/mcp-adapter-default-server\n  evidence: >-\n    POST https://www.mobia.com/wp-json/mcp/mcp-adapter-default-server ->\n    401 {\"code\":\"rest_forbidden\"}\n  note: >-\n    WordPress core authentication (login cookie + X-WP-Nonce, or an Application Password\n    over HTTP Basic). Not documented\
  \ by the provider; inferred from the standard\n    WordPress error contract returned by this host.\ncors:\n  allow_headers:\n  - Authorization\n  - X-WP-Nonce\n  - Content-Disposition\n  - Content-MD5\n  - Content-Type\n  expose_headers:\n  - X-WP-Total\n  - X-WP-TotalPages\n  - Link\n  evidence: observed on GET https://www.mobia.com/wp-json/wp/v2/news\ndocs: null\ndocs_note: The provider publishes no authentication reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microtransponder/refs/heads/main/authentication/microtransponder-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Neurotechnology
- Neuromodulation
- Stroke Rehabilitation
- Implantable Devices
- Life Sciences
- WordPress
- MCP
---
