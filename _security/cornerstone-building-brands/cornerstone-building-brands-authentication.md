---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
description: 'Two authentication postures on one host. The wp/v2 content read surface is anonymous — posts, pages, media, news, industry, leadership, categories, tags, news_category, news_solution, search, taxonomies, types and statuses all return HTTP 200 with no credential — while the MCP server routes, the WordPress Abilities registry and every administrative WordPress route (settings, menus, menu-items, block-types) require a bearer token or a WordPress session and answer 401. Probed rather than derived: the derived Content API declares no securitySchemes because its documented operations need none, so a spec-only derivation would have recorded "no authentication" and missed the OAuth server entirely. The company publishes no authentication documentation of its own; everything here is read from the discovery documents and observed responses. The separate Customer Portal (portal.cornerstonebuildingbrands.com) signs in with Microsoft Entra ID (MSAL) — observed in the portal''s public JavaScript
  bundle, not documented — and is out of scope for this profile.'
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Cornerstone Building Brands Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cornerstone Building Brands secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cornerstone Building Brands
provider_slug: cornerstone-building-brands
scheme_count: 2
schemes:
- applies_to: openapi/cornerstone-building-brands-content-api-openapi.yml
  description: The documented wp/v2 read operations require no credential. Verified anonymously on 2026-09-19 across all 14 collections in the derived spec (HTTP 200 each).
  name: none
  sources:
  - https://www.cornerstonebuildingbrands.com/wp-json/wp/v2/news?per_page=2
  type: none
- applies_to: https://www.cornerstonebuildingbrands.com/wp-json/mcp/mcp-oauth-server
  description: OAuth 2.1 authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported ["none"]), client-ID metadata documents in place of dynamic registration, single `mcp` scope, bearer token in the Authorization header. The 401 challenge carries a WWW-Authenticate header whose resource_metadata points at the RFC 9728 protected-resource document — the RFC 9728 discovery loop working as specified.
  flows:
  - authorizationUrl: https://www.cornerstonebuildingbrands.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://www.cornerstonebuildingbrands.com/oauth/token
    revocationUrl: https://www.cornerstonebuildingbrands.com/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://www.cornerstonebuildingbrands.com/oauth/token
  name: OAuth2
  sources:
  - https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server
  - https://www.cornerstonebuildingbrands.com/.well-known/oauth-protected-resource
  type: oauth2
slug: cornerstone-building-brands-authentication
source_filename: cornerstone-building-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: >-\n  https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server,\n  https://www.cornerstonebuildingbrands.com/.well-known/oauth-protected-resource, and live 200/401\n  responses observed on www.cornerstonebuildingbrands.com/wp-json on 2026-09-19\ndocs: null\ndescription: >-\n  Two authentication postures on one host. The wp/v2 content read surface is anonymous — posts, pages,\n  media, news, industry, leadership, categories, tags, news_category, news_solution, search, taxonomies,\n  types and statuses all return HTTP 200 with no credential — while the MCP server routes, the WordPress\n  Abilities registry and every administrative WordPress route (settings, menus, menu-items, block-types)\n  require a bearer token or a WordPress session and answer 401. Probed rather than derived: the derived\n  Content API declares no securitySchemes because its documented operations need none, so a spec-only\n  derivation\
  \ would have recorded \"no authentication\" and missed the OAuth server entirely. The company\n  publishes no authentication documentation of its own; everything here is read from the discovery\n  documents and observed responses. The separate Customer Portal (portal.cornerstonebuildingbrands.com)\n  signs in with Microsoft Entra ID (MSAL) — observed in the portal's public JavaScript bundle, not\n  documented — and is out of scope for this profile.\nsummary:\n  types: [none, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_read: true\n  pkce: S256\n  dynamic_client_registration: false\nschemes:\n- name: none\n  type: none\n  applies_to: openapi/cornerstone-building-brands-content-api-openapi.yml\n  description: >-\n    The documented wp/v2 read operations require no credential. Verified anonymously on 2026-09-19 across\n    all 14 collections in the derived spec (HTTP 200 each).\n  sources:\n  - https://www.cornerstonebuildingbrands.com/wp-json/wp/v2/news?per_page=2\n\
  - name: OAuth2\n  type: oauth2\n  applies_to: https://www.cornerstonebuildingbrands.com/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported\n    [\"none\"]), client-ID metadata documents in place of dynamic registration, single `mcp` scope, bearer\n    token in the Authorization header. The 401 challenge carries a WWW-Authenticate header whose\n    resource_metadata points at the RFC 9728 protected-resource document — the RFC 9728 discovery loop\n    working as specified.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.cornerstonebuildingbrands.com/oauth/authorize\n    tokenUrl: https://www.cornerstonebuildingbrands.com/oauth/token\n    revocationUrl: https://www.cornerstonebuildingbrands.com/oauth/revoke\n    refreshUrl: https://www.cornerstonebuildingbrands.com/oauth/token\n    scopes: [mcp]\n  sources:\n  - https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server\n\
  \  - https://www.cornerstonebuildingbrands.com/.well-known/oauth-protected-resource\nx-evidence:\n  fetched: '2026-09-19'\n  probes:\n  - url: https://www.cornerstonebuildingbrands.com/wp-json/wp/v2/posts?per_page=2\n    status: 200\n  - url: https://www.cornerstonebuildingbrands.com/wp-json/wp/v2/settings\n    status: 401\n  - url: https://www.cornerstonebuildingbrands.com/wp-json/mcp/mcp-oauth-server\n    method: POST tools/list\n    status: 401\n    www_authenticate: 'Bearer realm=\"https://www.cornerstonebuildingbrands.com\", resource_metadata=\"https://www.cornerstonebuildingbrands.com/.well-known/oauth-protected-resource\"'\n  - url: https://www.cornerstonebuildingbrands.com/oauth/token\n    method: POST (empty)\n    status: 400\n    body: '{\"error\":\"unsupported_grant_type\"}'\n  - url: https://www.cornerstonebuildingbrands.com/oauth/register\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornerstone-building-brands/refs/heads/main/authentication/cornerstone-building-brands-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Building Products
- Construction
- Manufacturing
- Building Materials
- MCP
- WordPress
- News
---
