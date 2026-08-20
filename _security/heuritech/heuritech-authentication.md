---
api_key_in: []
api_specs:
- filename: heuritech-posts-api-openapi.yml
  format: yaml
  label: Heuritech Posts API
  slug: heuritech-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-posts-api-openapi.yml
- filename: heuritech-pages-api-openapi.yml
  format: yaml
  label: Heuritech Pages API
  slug: heuritech-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-pages-api-openapi.yml
- filename: heuritech-media-api-openapi.yml
  format: yaml
  label: Heuritech Media API
  slug: heuritech-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-media-api-openapi.yml
- filename: heuritech-comments-api-openapi.yml
  format: yaml
  label: Heuritech Comments API
  slug: heuritech-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-comments-api-openapi.yml
- filename: heuritech-taxonomy-api-openapi.yml
  format: yaml
  label: Heuritech Taxonomy API
  slug: heuritech-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-taxonomy-api-openapi.yml
- filename: heuritech-users-api-openapi.yml
  format: yaml
  label: Heuritech Users API
  slug: heuritech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-users-api-openapi.yml
- filename: heuritech-search-api-openapi.yml
  format: yaml
  label: Heuritech Search API
  slug: heuritech-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-search-api-openapi.yml
- filename: heuritech-discovery-api-openapi.yml
  format: yaml
  label: Heuritech Discovery API
  slug: heuritech-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-discovery-api-openapi.yml
auth_types:
- none
- http
- oauth2
description: Heuritech has three distinct authentication postures, one per surface, and only two of them are publicly observable. The mechanical derive-authentication pass found no securitySchemes because the OpenAPI documents in this repo are API Evangelist derivations of an anonymously-readable WordPress REST surface, which declares none; the profile below was established by live probe instead.
kind: authentication
layout: security
method: probed
name: Heuritech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Heuritech secures its APIs with none, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Heuritech
provider_slug: heuritech
scheme_count: 3
schemes:
- description: 'Read operations on posts, pages, media, comments, categories, tags, users, search and the type/taxonomy/status discovery routes require no credentials. Verified live: HTTP 200 with X-WP-Total on every collection.'
  name: AnonymousRead
  source: https://heuritech.com/wp-json/wp/v2/posts
  surface: WordPress REST content API (wp/v2)
  type: none
  verified_status: 200
- authorization_endpoint: https://heuritech.com/wp-admin/authorize-application.php
  description: 'WordPress Application Passwords over HTTP Basic, the only authentication method the route index advertises. Also accepted: logged-in cookie plus an X-WP-Nonce header (the site''s Access-Control-Allow-Headers lists Authorization, X-WP-Nonce, Content-Disposition, Content-MD5 and Content-Type). Write operations are not modelled in this repo''s OpenAPI documents.'
  name: WordPressApplicationPassword
  scheme: basic
  source: https://heuritech.com/wp-json/ (authentication block)
  surface: WordPress REST content API (wp/v2) — write operations
  type: http
- description: 'OAuth 2.1 authorization code with PKCE guarding https://heuritech.com/wp-json/mcp/mcp-oauth-server. Public clients (token_endpoint_auth_methods_supported: none) with client-ID metadata documents instead of dynamic registration. Bearer token in the Authorization header. The 401 challenge is RFC 9728 compliant and names the protected-resource document.'
  detail: scopes/heuritech-scopes.yml
  flows:
  - authorizationUrl: https://heuritech.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: required
    revocationUrl: https://heuritech.com/oauth/revoke
    scopes: 1
    tokenUrl: https://heuritech.com/oauth/token
  issuer: https://heuritech.com
  name: HeuritechMCPOAuth
  source: https://heuritech.com/.well-known/oauth-authorization-server
  surface: Heuritech MCP server
  type: oauth2
slug: heuritech-authentication
source_filename: heuritech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  https://heuritech.com/wp-json/ (authentication block + live probes) and\n  https://heuritech.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Heuritech has three distinct authentication postures, one per surface, and only two of them are\n  publicly observable. The mechanical derive-authentication pass found no securitySchemes because the\n  OpenAPI documents in this repo are API Evangelist derivations of an anonymously-readable WordPress\n  REST surface, which declares none; the profile below was established by live probe instead.\nsummary:\n  types: [none, http, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    No API-key scheme is publicly documented anywhere on the Heuritech estate. The commercial product\n    API almost certainly has one, but Heuritech does not publish it, and guessing it would be fabrication.\nschemes:\n- name: AnonymousRead\n  type: none\n \
  \ surface: WordPress REST content API (wp/v2)\n  source: https://heuritech.com/wp-json/wp/v2/posts\n  description: >-\n    Read operations on posts, pages, media, comments, categories, tags, users, search and the\n    type/taxonomy/status discovery routes require no credentials. Verified live: HTTP 200 with\n    X-WP-Total on every collection.\n  verified_status: 200\n- name: WordPressApplicationPassword\n  type: http\n  scheme: basic\n  surface: WordPress REST content API (wp/v2) — write operations\n  source: https://heuritech.com/wp-json/ (authentication block)\n  authorization_endpoint: https://heuritech.com/wp-admin/authorize-application.php\n  description: >-\n    WordPress Application Passwords over HTTP Basic, the only authentication method the route index\n    advertises. Also accepted: logged-in cookie plus an X-WP-Nonce header (the site's\n    Access-Control-Allow-Headers lists Authorization, X-WP-Nonce, Content-Disposition, Content-MD5\n    and Content-Type). Write operations\
  \ are not modelled in this repo's OpenAPI documents.\n- name: HeuritechMCPOAuth\n  type: oauth2\n  surface: Heuritech MCP server\n  source: https://heuritech.com/.well-known/oauth-authorization-server\n  issuer: https://heuritech.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://heuritech.com/oauth/authorize\n    tokenUrl: https://heuritech.com/oauth/token\n    revocationUrl: https://heuritech.com/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    scopes: 1\n  description: >-\n    OAuth 2.1 authorization code with PKCE guarding https://heuritech.com/wp-json/mcp/mcp-oauth-server.\n    Public clients (token_endpoint_auth_methods_supported: none) with client-ID metadata documents\n    instead of dynamic registration. Bearer token in the Authorization header. The 401 challenge is\n    RFC 9728 compliant and names the protected-resource document.\n  detail: scopes/heuritech-scopes.yml\nundocumented:\n- surface: Heuritech Trend Data API\n  reason:\
  \ >-\n    Heuritech publishes no authentication documentation for its commercial API. The product page, the\n    pricing page and the FAQ all route prospective customers to a sales demo, and no developer portal,\n    API reference or key-management page exists on any Heuritech host. Recorded as undocumented rather\n    than assumed to be an API key.\n  probes:\n  - url: https://docs.heuritech.com/\n    status: 404\n  - url: https://developer.heuritech.com/\n    status: 404\n  - url: https://api.heuritech.com/docs\n    status: 404\nx-evidence:\n  fetched: '2026-08-17'\n  probes:\n  - url: https://heuritech.com/wp-json/wp/v2/posts?per_page=1\n    status: 200\n  - url: https://heuritech.com/wp-json/\n    status: 200\n  - url: https://heuritech.com/.well-known/oauth-authorization-server/\n    status: 200\n  - url: https://heuritech.com/wp-json/mcp/mcp-oauth-server\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/authentication/heuritech-authentication.yml
summary_line: none/http/oauth2 · 3 schemes
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Machine-Learning
- Fashion
- Trend Forecasting
- Demand Forecasting
- Retail
- Luxury
- Market Intelligence
- Consumer Insights
- Social Media Analytics
- Content
---
