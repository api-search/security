---
anonymous_access: true
api_key_in: []
api_specs:
- filename: 1000satellitescoworking-content-api-openapi.yml
  format: yaml
  label: 1000 Satellites Content API (WordPress REST wp/v2)
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1000satellitescoworking/refs/heads/main/openapi/1000satellitescoworking-content-api-openapi.yml
auth_types:
- none
- oauth2
description: '1000 Satellites has two authentication postures on one host, and they are opposites. The wp/v2 content read surface is fully anonymous — ten resources return 200 with no credential — while the MCP server and every administrative WordPress route require a bearer token or a WordPress session. This artifact was probed rather than derived: the derived Content API declares no securitySchemes precisely because its documented operations need none, so a spec-only derivation would have recorded "no authentication" and missed the OAuth server entirely.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 1000Satellitescoworking Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 1000 Satellites secures its APIs with none and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 1000 Satellites
provider_slug: 1000satellitescoworking
scheme_count: 3
schemes:
- applies_to: openapi/1000satellitescoworking-content-api-openapi.yml
  description: 'The documented wp/v2 read operations require no credential. Verified anonymously on 2026-09-05: /wp/v2/posts, /pages, /media, /categories, /tags, /comments, /types, /taxonomies, /statuses and /search all returned HTTP 200.'
  name: none
  sources:
  - https://1000satellites.de/wp-json/wp/v2/posts
  type: none
- applies_to: https://1000satellites.de/wp-json/mcp/mcp-oauth-server
  description: OAuth 2.1 authorization code with PKCE (S256), public clients, single `mcp` scope, bearer token in the Authorization header. The 401 challenge carries a WWW-Authenticate header pointing at the RFC 9728 protected-resource document, which is the RFC 9728 discovery flow working as specified.
  detail: scopes/1000satellitescoworking-scopes.yml
  flows:
  - authorizationUrl: https://1000satellites.de/oauth/authorize
    client_registration: No RFC 7591 dynamic client registration endpoint is advertised. The metadata sets client_id_metadata_document_supported true, so a client identifies itself with a client-ID metadata document URL rather than a pre-registered client_id.
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://1000satellites.de/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://1000satellites.de/oauth/token
    token_endpoint_auth_methods_supported:
    - none
  name: OAuth2
  sources:
  - https://1000satellites.de/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: /wp/v2/users, /wp/v2/settings, /wp/v2/themes, /wp/v2/plugins, /wp/v2/menus, /wp/v2/block-types, /wp-abilities/v1/abilities and every write method on the wp/v2 routes
  description: Standard WordPress authentication — a logged-in cookie plus X-WP-Nonce, or Application Passwords over HTTP Basic. Anonymous requests to these routes return 401 rest_forbidden. Not documented by the provider; recorded from the observed 401s and from the Access-Control-Allow-Headers response header, which advertises Authorization and X-WP-Nonce.
  name: WordPressSession
  scheme: cookie-or-basic
  sources:
  - https://1000satellites.de/wp-json/wp/v2/users
  type: http
slug: 1000satellitescoworking-authentication
source_filename: 1000satellitescoworking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://1000satellites.de/.well-known/oauth-authorization-server,\n  https://1000satellites.de/.well-known/oauth-protected-resource, and live 200/401 responses observed on\n  1000satellites.de/wp-json\ndescription: >-\n  1000 Satellites has two authentication postures on one host, and they are opposites. The wp/v2 content\n  read surface is fully anonymous — ten resources return 200 with no credential — while the MCP server and\n  every administrative WordPress route require a bearer token or a WordPress session. This artifact was\n  probed rather than derived: the derived Content API declares no securitySchemes precisely because its\n  documented operations need none, so a spec-only derivation would have recorded \"no authentication\" and\n  missed the OAuth server entirely.\nsummary:\n  types: [none, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_read: true\nschemes:\n- name: none\n  type:\
  \ none\n  applies_to: openapi/1000satellitescoworking-content-api-openapi.yml\n  description: >-\n    The documented wp/v2 read operations require no credential. Verified anonymously on 2026-09-05:\n    /wp/v2/posts, /pages, /media, /categories, /tags, /comments, /types, /taxonomies, /statuses and /search\n    all returned HTTP 200.\n  sources: [https://1000satellites.de/wp-json/wp/v2/posts]\n- name: OAuth2\n  type: oauth2\n  applies_to: https://1000satellites.de/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 authorization code with PKCE (S256), public clients, single `mcp` scope, bearer token in the\n    Authorization header. The 401 challenge carries a WWW-Authenticate header pointing at the RFC 9728\n    protected-resource document, which is the RFC 9728 discovery flow working as specified.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://1000satellites.de/oauth/authorize\n    tokenUrl: https://1000satellites.de/oauth/token\n    revocationUrl: https://1000satellites.de/oauth/revoke\n\
  \    scopes: [mcp]\n    pkce: S256\n    token_endpoint_auth_methods_supported: [none]\n    client_registration: >-\n      No RFC 7591 dynamic client registration endpoint is advertised. The metadata sets\n      client_id_metadata_document_supported true, so a client identifies itself with a client-ID metadata\n      document URL rather than a pre-registered client_id.\n  detail: scopes/1000satellitescoworking-scopes.yml\n  sources: [https://1000satellites.de/.well-known/oauth-authorization-server]\n- name: WordPressSession\n  type: http\n  scheme: cookie-or-basic\n  applies_to: >-\n    /wp/v2/users, /wp/v2/settings, /wp/v2/themes, /wp/v2/plugins, /wp/v2/menus, /wp/v2/block-types,\n    /wp-abilities/v1/abilities and every write method on the wp/v2 routes\n  description: >-\n    Standard WordPress authentication — a logged-in cookie plus X-WP-Nonce, or Application Passwords over\n    HTTP Basic. Anonymous requests to these routes return 401 rest_forbidden. Not documented by the\n    provider;\
  \ recorded from the observed 401s and from the Access-Control-Allow-Headers response header,\n    which advertises Authorization and X-WP-Nonce.\n  sources: [https://1000satellites.de/wp-json/wp/v2/users]\nnotes:\n- >-\n  No API key scheme of any kind exists on this provider. There is no developer portal, no key issuance\n  page, and no sign-up flow that yields a credential — the sign-up surface on the site books workspace,\n  not API access.\nx-evidence:\n  fetched: '2026-09-05'\n  probes:\n  - {url: 'https://1000satellites.de/wp-json/wp/v2/posts?per_page=1', status: 200}\n  - {url: 'https://1000satellites.de/wp-json/wp/v2/users?per_page=1', status: 401}\n  - {url: 'https://1000satellites.de/wp-json/wp-abilities/v1/abilities', status: 401}\n  - {url: 'https://1000satellites.de/wp-json/mcp/mcp-oauth-server', method: POST tools/list, status: 401}\n  - {url: 'https://1000satellites.de/.well-known/oauth-authorization-server', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1000satellitescoworking/refs/heads/main/authentication/1000satellitescoworking-authentication.yml
summary_line: none/oauth2 · 3 schemes
tags:
- Company
- Coworking
- Flexible Workspace
- Real Estate
- Office Space
- Workplace
- Meeting Rooms
- Germany
- Content
- MCP
---
