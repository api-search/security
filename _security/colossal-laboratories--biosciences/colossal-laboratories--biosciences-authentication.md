---
api_key_in: []
api_specs:
- filename: colossal-laboratories--biosciences-comments-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Comments API
  slug: colossal-laboratories--biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-comments-api-openapi.yml
- filename: colossal-laboratories--biosciences-discovery-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Discovery API
  slug: colossal-laboratories--biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-discovery-api-openapi.yml
- filename: colossal-laboratories--biosciences-media-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Media API
  slug: colossal-laboratories--biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-media-api-openapi.yml
- filename: colossal-laboratories--biosciences-pages-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Pages API
  slug: colossal-laboratories--biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-pages-api-openapi.yml
- filename: colossal-laboratories--biosciences-posts-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Posts API
  slug: colossal-laboratories--biosciences-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-posts-api-openapi.yml
- filename: colossal-laboratories--biosciences-search-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Search API
  slug: colossal-laboratories--biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-search-api-openapi.yml
- filename: colossal-laboratories--biosciences-settings-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Settings API
  slug: colossal-laboratories--biosciences-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-settings-api-openapi.yml
- filename: colossal-laboratories--biosciences-taxonomy-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Taxonomy API
  slug: colossal-laboratories--biosciences-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-taxonomy-api-openapi.yml
- filename: colossal-laboratories--biosciences-users-api-openapi.yml
  format: yaml
  label: Colossal Laboratories & Biosciences Users API
  slug: colossal-laboratories--biosciences-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/openapi/colossal-laboratories--biosciences-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Colossal Laboratories  Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Colossal Laboratories & Biosciences secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Colossal Laboratories & Biosciences
provider_slug: colossal-laboratories--biosciences
scheme_count: 2
schemes:
- applies_to: every create / replace / update / delete operation in the derived OpenAPI
  description: WordPress Application Passwords, advertised by the site at https://colossal.com/wp-json/ under authentication.application-passwords; authorization endpoint https://colossal.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  issuance: Self-service only for accounts that already hold a colossal.com WordPress login. No third party can obtain one, so in practice this API is read-only to everyone outside Colossal.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/colossal-laboratories--biosciences-content-openapi.yml
  - https://colossal.com/wp-json/ (authentication.application-passwords)
  type: http
- description: The browser path — a logged-in WordPress cookie plus an X-WP-Nonce request header. Not usable by a server-to-server client. Evidenced by the CORS preflight allowlist, which includes X-WP-Nonce.
  name: cookieNonce
  observed: 'access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'
  type: cookie
slug: colossal-laboratories--biosciences-authentication
source_filename: colossal-laboratories--biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: >-\n  openapi/colossal-laboratories--biosciences-content-openapi.yml (derived from\n  https://colossal.com/wp-json/) plus live anonymous probes of the wp/v2, mcp and\n  wp-abilities/v1 namespaces, 2026-08-09\ndocs: null\ndocs_note: >-\n  Colossal publishes no authentication documentation, because it publishes no developer\n  documentation at all. Everything below was observed, not read.\nsummary:\n  types:\n  - http\n  anonymous_read: true\n  oauth2: false\n  openid_connect: false\n  api_keys: false\n  mutual_tls: false\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords, advertised by the site at https://colossal.com/wp-json/\n    under authentication.application-passwords; authorization endpoint\n    https://colossal.com/wp-admin/authorize-application.php. Read operations on wp/v2 are\n    anonymous.\n  applies_to: every create / replace / update / delete\
  \ operation in the derived OpenAPI\n  issuance: >-\n    Self-service only for accounts that already hold a colossal.com WordPress login. No third\n    party can obtain one, so in practice this API is read-only to everyone outside Colossal.\n  sources:\n  - openapi/colossal-laboratories--biosciences-content-openapi.yml\n  - https://colossal.com/wp-json/ (authentication.application-passwords)\n- name: cookieNonce\n  type: cookie\n  description: >-\n    The browser path — a logged-in WordPress cookie plus an X-WP-Nonce request header. Not\n    usable by a server-to-server client. Evidenced by the CORS preflight allowlist, which\n    includes X-WP-Nonce.\n  observed: 'access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'\nanonymous_access:\n  readable_without_credentials:\n  - /wp/v2/posts (200, X-WP-Total 238)\n  - /wp/v2/pages (200, X-WP-Total 59)\n  - /wp/v2/media (200, X-WP-Total 990)\n  - /wp/v2/categories (200, 15)\n  - /wp/v2/tags (200,\
  \ 156)\n  - /wp/v2/users (200, 8)\n  - /wp/v2/comments (200, 0)\n  - /wp/v2/search (200, 297)\n  - /wp/v2/taxonomies (200)\n  - /wp/v2/statuses (200)\n  gated_to_anonymous:\n  - {path: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {path: /wp-json/mcp/mcp-adapter-default-server, status: 401, code: rest_forbidden, method: 'JSON-RPC tools/list and initialize'}\n  - {path: /wp-json/wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\ndiscovery:\n  oauth_authorization_server: {path: /.well-known/oauth-authorization-server, status: 404}\n  oauth_protected_resource: {path: /.well-known/oauth-protected-resource, status: 404}\n  openid_configuration: {path: /.well-known/openid-configuration, status: 404}\n  note: >-\n    No OAuth or OIDC discovery document is served, so the MCP endpoint's 401 carries no\n    machine-readable challenge an agent could follow. No OAuthScopes artifact is emitted —\n    there is no oauth2 securityScheme and no documented scope vocabulary to derive\
  \ one from.\nobservations:\n- finding: anonymous user enumeration\n  detail: >-\n    GET /wp/v2/users returns all 8 contributor accounts — display name, slug and public\n    author-archive URL — with no credentials. This is default WordPress behaviour rather than a\n    Colossal decision, but it is the standard first step of a WordPress credential-stuffing\n    attempt and is worth Colossal's attention. API Evangelist records the shape and count only\n    and does not republish the identities.\n  status: 200\n- finding: no vulnerability-disclosure channel\n  detail: >-\n    /.well-known/security.txt and /security.txt both 404, and no bug-bounty or disclosure page\n    exists, so there is no published route to report the item above. See\n    security/colossal-laboratories--biosciences-domain-security.yml.\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossal-laboratories--biosciences/refs/heads/main/authentication/colossal-laboratories--biosciences-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Biotechnology
- Genomics
- Genetic Engineering
- Synthetic Biology
- De-Extinction
- Conservation
- Wildlife
- Life Sciences
- CRISPR
- Research
- Content
---
