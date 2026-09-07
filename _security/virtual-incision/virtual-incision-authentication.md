---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: virtual-incision-posts-api-openapi.yml
  format: yaml
  label: Virtual Incision News Posts API
  slug: virtual-incision-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-posts-api-openapi.yml
- filename: virtual-incision-pages-api-openapi.yml
  format: yaml
  label: Virtual Incision Pages API
  slug: virtual-incision-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-pages-api-openapi.yml
- filename: virtual-incision-media-api-openapi.yml
  format: yaml
  label: Virtual Incision Media API
  slug: virtual-incision-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-media-api-openapi.yml
- filename: virtual-incision-events-api-openapi.yml
  format: yaml
  label: Virtual Incision Events API
  slug: virtual-incision-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-events-api-openapi.yml
- filename: virtual-incision-careers-api-openapi.yml
  format: yaml
  label: Virtual Incision Careers API
  slug: virtual-incision-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-careers-api-openapi.yml
- filename: virtual-incision-taxonomy-api-openapi.yml
  format: yaml
  label: Virtual Incision Taxonomy API
  slug: virtual-incision-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-taxonomy-api-openapi.yml
- filename: virtual-incision-people-api-openapi.yml
  format: yaml
  label: Virtual Incision People API
  slug: virtual-incision-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-people-api-openapi.yml
- filename: virtual-incision-search-api-openapi.yml
  format: yaml
  label: Virtual Incision Search API
  slug: virtual-incision-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-search-api-openapi.yml
- filename: virtual-incision-discovery-api-openapi.yml
  format: yaml
  label: Virtual Incision Discovery API
  slug: virtual-incision-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/openapi/virtual-incision-discovery-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Virtual Incision Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virtual Incision secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Virtual Incision
provider_slug: virtual-incision
scheme_count: 3
schemes:
- description: WordPress Application Passwords over HTTP Basic. Issued at https://virtualincision.com/wp-admin/authorize-application.php (advertised by the wp-json root `authentication` block).
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/virtual-incision-careers-api-openapi.yml
  - openapi/virtual-incision-discovery-api-openapi.yml
  - openapi/virtual-incision-events-api-openapi.yml
  - openapi/virtual-incision-media-api-openapi.yml
  - openapi/virtual-incision-pages-api-openapi.yml
  - openapi/virtual-incision-people-api-openapi.yml
  - openapi/virtual-incision-posts-api-openapi.yml
  - openapi/virtual-incision-search-api-openapi.yml
  - openapi/virtual-incision-taxonomy-api-openapi.yml
  type: http
- description: Logged-in WordPress cookie plus an X-WP-Nonce header — first-party browser context only.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/virtual-incision-careers-api-openapi.yml
  - openapi/virtual-incision-discovery-api-openapi.yml
  - openapi/virtual-incision-events-api-openapi.yml
  - openapi/virtual-incision-media-api-openapi.yml
  - openapi/virtual-incision-pages-api-openapi.yml
  - openapi/virtual-incision-people-api-openapi.yml
  - openapi/virtual-incision-posts-api-openapi.yml
  - openapi/virtual-incision-search-api-openapi.yml
  - openapi/virtual-incision-taxonomy-api-openapi.yml
  type: apiKey
- applies_to: https://virtualincision.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://virtualincision.com/oauth/authorize
  client_id_metadata_document_supported: true
  description: OAuth 2.1 authorization server advertised by an RFC 8414 document at the domain root and referenced by an RFC 9728 protected-resource document. Public client, PKCE required, one scope. This scheme does NOT appear in any OpenAPI in this repo because it governs the MCP endpoint, not the wp/v2 REST surface.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  pkce:
  - S256
  revocation_endpoint: https://virtualincision.com/oauth/revoke
  scopes:
  - mcp
  sources:
  - well-known/virtual-incision-oauth-authorization-server.json
  - well-known/virtual-incision-oauth-protected-resource.json
  token_endpoint: https://virtualincision.com/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: virtual-incision-authentication
source_filename: virtual-incision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/*.yml securitySchemes (derived) + https://virtualincision.com/wp-json/ `authentication` block +\n  https://virtualincision.com/.well-known/oauth-authorization-server + https://virtualincision.com/.well-known/oauth-protected-resource\n  (probed 2026-09-04)\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Issued at https://virtualincision.com/wp-admin/authorize-application.php\n    (advertised by the wp-json root `authentication` block).\n  sources:\n  - openapi/virtual-incision-careers-api-openapi.yml\n  - openapi/virtual-incision-discovery-api-openapi.yml\n  - openapi/virtual-incision-events-api-openapi.yml\n  - openapi/virtual-incision-media-api-openapi.yml\n  - openapi/virtual-incision-pages-api-openapi.yml\n  - openapi/virtual-incision-people-api-openapi.yml\n\
  \  - openapi/virtual-incision-posts-api-openapi.yml\n  - openapi/virtual-incision-search-api-openapi.yml\n  - openapi/virtual-incision-taxonomy-api-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: Logged-in WordPress cookie plus an X-WP-Nonce header — first-party browser context only.\n  sources:\n  - openapi/virtual-incision-careers-api-openapi.yml\n  - openapi/virtual-incision-discovery-api-openapi.yml\n  - openapi/virtual-incision-events-api-openapi.yml\n  - openapi/virtual-incision-media-api-openapi.yml\n  - openapi/virtual-incision-pages-api-openapi.yml\n  - openapi/virtual-incision-people-api-openapi.yml\n  - openapi/virtual-incision-posts-api-openapi.yml\n  - openapi/virtual-incision-search-api-openapi.yml\n  - openapi/virtual-incision-taxonomy-api-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  authorization_endpoint: https://virtualincision.com/oauth/authorize\n  token_endpoint: https://virtualincision.com/oauth/token\n\
  \  revocation_endpoint: https://virtualincision.com/oauth/revoke\n  pkce:\n  - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  client_id_metadata_document_supported: true\n  scopes:\n  - mcp\n  applies_to: https://virtualincision.com/wp-json/mcp/mcp-oauth-server\n  description: OAuth 2.1 authorization server advertised by an RFC 8414 document at the domain root and referenced\n    by an RFC 9728 protected-resource document. Public client, PKCE required, one scope. This scheme does NOT appear\n    in any OpenAPI in this repo because it governs the MCP endpoint, not the wp/v2 REST surface.\n  sources:\n  - well-known/virtual-incision-oauth-authorization-server.json\n  - well-known/virtual-incision-oauth-protected-resource.json\nanonymous_read:\n  supported: true\n  detail: Every wp/v2 content collection (posts, pages, media, event, jobpost and their taxonomies, categories,\n    tags, users, search, types, statuses, comments) returned\
  \ HTTP 200 to an unauthenticated GET. settings, menus,\n    plugins and themes returned 401.\n  evidence: https://virtualincision.com/wp-json/wp/v2/posts?per_page=1 -> 200; https://virtualincision.com/wp-json/wp/v2/settings\n    -> 401\ndocs: https://virtualincision.com/wp-admin/authorize-application.php\ndocs_note: Virtual Incision publishes NO authentication documentation of its own — there is no developer portal\n  or docs site. The Application Password authorize screen is WordPress core, advertised by the `authentication`\n  block of https://virtualincision.com/wp-json/, and requires an existing WordPress login. Nothing on this host\n  is obtainable by a member of the public.\nnote: 'Three distinct schemes on one host: anonymous read for wp/v2 content, WordPress Application Passwords (HTTP\n  Basic) or cookie+X-WP-Nonce for wp/v2 writes, and OAuth 2.1 bearer with scope \"mcp\" for the MCP endpoint. An agent\n  must know which surface it is on before it picks a credential.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/authentication/virtual-incision-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Medical Devices
- Surgical Robotics
- Robotics
- Healthcare
- Health
- Life Sciences
- Medical Technology
- Content
- News
- Careers
- Events
- Model Context Protocol
---
