---
api_key_in:
- header
api_specs:
- filename: livekindly-brands-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Brands API
  slug: livekindly-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-brands-api-openapi.yml
- filename: livekindly-careers-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Careers API
  slug: livekindly-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-careers-api-openapi.yml
- filename: livekindly-comments-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Comments API
  slug: livekindly-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-comments-api-openapi.yml
- filename: livekindly-discovery-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Discovery API
  slug: livekindly-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-discovery-api-openapi.yml
- filename: livekindly-media-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Media API
  slug: livekindly-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-media-api-openapi.yml
- filename: livekindly-pages-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Pages API
  slug: livekindly-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-pages-api-openapi.yml
- filename: livekindly-partners-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Partners API
  slug: livekindly-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-partners-api-openapi.yml
- filename: livekindly-posts-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Posts API
  slug: livekindly-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-posts-api-openapi.yml
- filename: livekindly-search-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Search API
  slug: livekindly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-search-api-openapi.yml
- filename: livekindly-settings-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Settings API
  slug: livekindly-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-settings-api-openapi.yml
- filename: livekindly-taxonomy-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Taxonomy API
  slug: livekindly-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-taxonomy-api-openapi.yml
- filename: livekindly-users-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Users API
  slug: livekindly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-users-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Livekindly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LIVEKINDLY secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LIVEKINDLY
provider_slug: livekindly
scheme_count: 3
schemes:
- applies_to: livekindly:content
  description: WordPress Application Passwords over HTTP Basic. Issued per-user from https://thelivekindlyco.com/wp-admin/authorize-application.php. Required for every write operation on wp/v2 and for the routes that return author or settings data.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/livekindly-content-openapi.yml
  type: http
- applies_to: livekindly:content
  description: Logged-in cookie authentication paired with an X-WP-Nonce header. Browser/admin context only; not usable by a server-side or agent client.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/livekindly-content-openapi.yml
  type: apiKey
- applies_to: livekindly:mcp
  artifact: scopes/livekindly-scopes.yml
  description: OAuth 2.0 authorization code + PKCE (S256 required) protecting the WordPress MCP Adapter endpoints. Public clients only — token_endpoint_auth_methods is [none] — and client identity is expressed with a client-ID metadata document rather than dynamic client registration.
  flows:
  - authorizationUrl: https://thelivekindlyco.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://thelivekindlyco.com/oauth/token
    scopes:
      mcp: The single scope the authorization server advertises.
    tokenUrl: https://thelivekindlyco.com/oauth/token
  issuer: https://thelivekindlyco.com
  name: mcp-oauth
  revocation_endpoint: https://thelivekindlyco.com/oauth/revoke
  scope_count: 1
  sources:
  - https://thelivekindlyco.com/.well-known/oauth-authorization-server
  - https://thelivekindlyco.com/.well-known/oauth-protected-resource
  type: oauth2
slug: livekindly-authentication
source_filename: livekindly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/livekindly-content-openapi.yml\nalso_source: https://thelivekindlyco.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  LIVEKINDLY publishes no developer or authentication documentation. The baseline below was\n  derived mechanically from the OpenAPI in this repo (itself derived from the live\n  https://thelivekindlyco.com/wp-json/ route index) and then upgraded with the OAuth 2.0\n  authorization-server metadata LIVEKINDLY actually serves at /.well-known/, which the spec\n  derivation cannot see.\nnote: >-\n  Two independent authentication models coexist on thelivekindlyco.com. (1) The wp/v2 content API\n  is ANONYMOUS for reads — every collection in openapi/ returned 200 with no credential — and\n  falls back to WordPress Application Passwords over HTTP Basic (or logged-in cookie +\n  X-WP-Nonce in a browser) for writes. (2) The MCP endpoints are protected by a real OAuth 2.0\n  authorization\
  \ server with PKCE and a single \"mcp\" scope. Neither model is documented by\n  LIVEKINDLY anywhere a developer would find it.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  anonymous_read: true\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords over HTTP Basic. Issued per-user from\n    https://thelivekindlyco.com/wp-admin/authorize-application.php. Required for every write\n    operation on wp/v2 and for the routes that return author or settings data.\n  applies_to: livekindly:content\n  sources:\n  - openapi/livekindly-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: >-\n    Logged-in cookie authentication paired with an X-WP-Nonce header. Browser/admin context only;\n    not usable by a server-side or agent client.\n  applies_to: livekindly:content\n  sources:\n  - openapi/livekindly-content-openapi.yml\n\
  - name: mcp-oauth\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization code + PKCE (S256 required) protecting the WordPress MCP Adapter\n    endpoints. Public clients only — token_endpoint_auth_methods is [none] — and client identity\n    is expressed with a client-ID metadata document rather than dynamic client registration.\n  applies_to: livekindly:mcp\n  issuer: https://thelivekindlyco.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thelivekindlyco.com/oauth/authorize\n    tokenUrl: https://thelivekindlyco.com/oauth/token\n    refreshUrl: https://thelivekindlyco.com/oauth/token\n    scopes:\n      mcp: The single scope the authorization server advertises.\n  revocation_endpoint: https://thelivekindlyco.com/oauth/revoke\n  scope_count: 1\n  artifact: scopes/livekindly-scopes.yml\n  sources:\n  - https://thelivekindlyco.com/.well-known/oauth-authorization-server\n  - https://thelivekindlyco.com/.well-known/oauth-protected-resource\nanonymous_access:\n\
  \  content_api:\n    readable: true\n    observed:\n    - {operation: getPosts, url: 'https://thelivekindlyco.com/wp-json/wp/v2/posts?per_page=1', status: 200, x_wp_total: 39}\n    - {operation: getPages, status: 200, x_wp_total: 19}\n    - {operation: getBrand, status: 200, x_wp_total: 4}\n    - {operation: getPartner, status: 200, x_wp_total: 4}\n    - {operation: getJob, status: 200, x_wp_total: 6}\n    - {operation: getMedia, status: 200, x_wp_total: 1145}\n    - {operation: getCategories, status: 200, x_wp_total: 3}\n    denied:\n    - {operation: getUsers, status: 403, note: 'blocked at the edge by the Sucuri WAF (Block ID UAT007), which returns an HTML interstitial rather than the WordPress JSON error envelope — not an application permission check'}\n  mcp:\n    readable: false\n    challenge: 'WWW-Authenticate: Bearer realm=\"https://thelivekindlyco.com\", resource_metadata=\"https://thelivekindlyco.com/.well-known/oauth-protected-resource\"'\n    challenge_note: >-\n      The\
  \ 401 carries a correct RFC 9728 bearer challenge pointing at the protected-resource\n      metadata, so an MCP client can discover the authorization server from the failure alone\n      without any documentation. This is the strongest single piece of auth ergonomics on the\n      whole LIVEKINDLY surface.\n    observed:\n    - {endpoint: /wp-json/mcp/mcp-oauth-server, method: tools/list, status: 401, code: mcp_unauthorized}\n    - {endpoint: /wp-json/mcp/mcp-adapter-default-server, method: tools/list, status: 401, code: rest_forbidden}\n    - {endpoint: /wp-json/wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\ntransport_security:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    No Strict-Transport-Security header is set on thelivekindlyco.com, so a first plaintext\n    request is not protected by HSTS. A Content-Security-Policy of upgrade-insecure-requests is\n    present instead. See security/livekindly-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/authentication/livekindly-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Food and Beverage
- Plant-Based
- Alternative Protein
- Consumer Packaged Goods
- Sustainability
- Manufacturing
- Retail
- Content
- Newsroom
---
