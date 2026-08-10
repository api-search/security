---
api_key_in: []
api_specs:
- filename: vestaron-comments-api-openapi.yml
  format: yaml
  label: Vestaron Comments API
  slug: vestaron-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-comments-api-openapi.yml
- filename: vestaron-discovery-api-openapi.yml
  format: yaml
  label: Vestaron Discovery API
  slug: vestaron-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-discovery-api-openapi.yml
- filename: vestaron-media-api-openapi.yml
  format: yaml
  label: Vestaron Media API
  slug: vestaron-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-media-api-openapi.yml
- filename: vestaron-pages-api-openapi.yml
  format: yaml
  label: Vestaron Pages API
  slug: vestaron-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-pages-api-openapi.yml
- filename: vestaron-posts-api-openapi.yml
  format: yaml
  label: Vestaron Posts API
  slug: vestaron-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-posts-api-openapi.yml
- filename: vestaron-search-api-openapi.yml
  format: yaml
  label: Vestaron Search API
  slug: vestaron-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-search-api-openapi.yml
- filename: vestaron-settings-api-openapi.yml
  format: yaml
  label: Vestaron Settings API
  slug: vestaron-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-settings-api-openapi.yml
- filename: vestaron-taxonomy-api-openapi.yml
  format: yaml
  label: Vestaron Taxonomy API
  slug: vestaron-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-taxonomy-api-openapi.yml
- filename: vestaron-users-api-openapi.yml
  format: yaml
  label: Vestaron Users API
  slug: vestaron-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-users-api-openapi.yml
auth_types:
- none
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Vestaron Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vestaron secures its APIs with none, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vestaron
provider_slug: vestaron
scheme_count: 3
schemes:
- applies_to: https://vestaron.com/wp-json/wp/v2
  description: 'Read operations on the wp/v2 content collections require no credentials. Probed 2026-08-05: /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags, /wp/v2/comments, /wp/v2/search and /wp/v2/types all returned 200 anonymously.'
  name: anonymous
  sources:
  - openapi/vestaron-content-openapi.yml
  type: none
- applies_to: https://vestaron.com/wp-json/wp/v2
  description: WordPress Application Passwords over HTTP Basic. The application-password routes are registered on vestaron.com (/wp/v2/users/{user_id}/application-passwords), but the site's route-discovery document reports an empty "authentication" object, so no authentication scheme is advertised for discovery. /wp/v2/users and /wp/v2/settings return 401 to anonymous callers, as do all write operations.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/vestaron-content-openapi.yml
  type: http
- applies_to: https://vestaron.com/wp-json/mcp/mcp-oauth-server
  description: 'OAuth 2.1 authorization-code with mandatory PKCE (S256), public clients (token_endpoint_auth_methods_supported: none), refresh tokens, client-ID metadata documents, bearer token in the Authorization header. Single scope "mcp". Advertised anonymously via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata.'
  flows:
  - authorizationUrl: https://vestaron.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://vestaron.com/oauth/revoke
    scopes: 1
    tokenUrl: https://vestaron.com/oauth/token
  name: mcp-oauth
  sources:
  - well-known/vestaron-oauth-authorization-server.json
  - well-known/vestaron-oauth-protected-resource.json
  type: oauth2
slug: vestaron-authentication
source_filename: vestaron-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: openapi/vestaron-content-openapi.yml + https://vestaron.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - none\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Vestaron publishes no developer authentication documentation. The profile below is what the\n    two live machine-readable surfaces on vestaron.com actually declare: anonymous read on the\n    WordPress content API, HTTP Basic (Application Passwords) for writes, and OAuth 2.1 + PKCE\n    for the MCP endpoint.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: https://vestaron.com/wp-json/wp/v2\n  description: >-\n    Read operations on the wp/v2 content collections require no credentials. Probed 2026-08-05:\n    /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags, /wp/v2/comments,\n    /wp/v2/search and /wp/v2/types all returned 200 anonymously.\n  sources:\n  - openapi/vestaron-content-openapi.yml\n\
  - name: applicationPassword\n  type: http\n  scheme: basic\n  applies_to: https://vestaron.com/wp-json/wp/v2\n  description: >-\n    WordPress Application Passwords over HTTP Basic. The application-password routes are\n    registered on vestaron.com (/wp/v2/users/{user_id}/application-passwords), but the site's\n    route-discovery document reports an empty \"authentication\" object, so no authentication\n    scheme is advertised for discovery. /wp/v2/users and /wp/v2/settings return 401 to anonymous\n    callers, as do all write operations.\n  sources:\n  - openapi/vestaron-content-openapi.yml\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://vestaron.com/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 authorization-code with mandatory PKCE (S256), public clients\n    (token_endpoint_auth_methods_supported: none), refresh tokens, client-ID metadata documents,\n    bearer token in the Authorization header. Single scope \"mcp\". Advertised anonymously via\n    RFC\
  \ 8414 authorization-server metadata and RFC 9728 protected-resource metadata.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vestaron.com/oauth/authorize\n    tokenUrl: https://vestaron.com/oauth/token\n    revocationUrl: https://vestaron.com/oauth/revoke\n    scopes: 1\n  sources:\n  - well-known/vestaron-oauth-authorization-server.json\n  - well-known/vestaron-oauth-protected-resource.json\nscopes_artifact: scopes/vestaron-scopes.yml\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://vestaron.com/wp-json/wp/v2/posts?per_page=1\n    http_status: 200\n  - url: https://vestaron.com/wp-json/wp/v2/users?per_page=1\n    http_status: 401\n  - url: https://vestaron.com/wp-json/wp/v2/settings\n    http_status: 401\n  - url: https://vestaron.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/authentication/vestaron-authentication.yml
summary_line: none/http/oauth2 · 3 schemes
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Crop Protection
- Bioinsecticides
- Peptides
- Biologicals
- Sustainability
- Pollinator Safety
- Life Sciences
- Content
---
