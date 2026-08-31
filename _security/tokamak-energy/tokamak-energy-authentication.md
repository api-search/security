---
api_key_in: []
api_specs:
- filename: tokamak-energy-posts-api-openapi.yml
  format: yaml
  label: Tokamak Energy Posts API
  slug: tokamak-energy-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-posts-api-openapi.yml
- filename: tokamak-energy-pages-api-openapi.yml
  format: yaml
  label: Tokamak Energy Pages API
  slug: tokamak-energy-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-pages-api-openapi.yml
- filename: tokamak-energy-media-api-openapi.yml
  format: yaml
  label: Tokamak Energy Media API
  slug: tokamak-energy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-media-api-openapi.yml
- filename: tokamak-energy-area-items-api-openapi.yml
  format: yaml
  label: Tokamak Energy Area Items API
  slug: tokamak-energy-area-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-area-items-api-openapi.yml
- filename: tokamak-energy-taxonomy-api-openapi.yml
  format: yaml
  label: Tokamak Energy Taxonomy API
  slug: tokamak-energy-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-taxonomy-api-openapi.yml
- filename: tokamak-energy-search-api-openapi.yml
  format: yaml
  label: Tokamak Energy Search API
  slug: tokamak-energy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-search-api-openapi.yml
- filename: tokamak-energy-authors-api-openapi.yml
  format: yaml
  label: Tokamak Energy Authors API
  slug: tokamak-energy-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-authors-api-openapi.yml
- filename: tokamak-energy-discovery-api-openapi.yml
  format: yaml
  label: Tokamak Energy Discovery API
  slug: tokamak-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-discovery-api-openapi.yml
- filename: tokamak-energy-oembed-api-openapi.yml
  format: yaml
  label: Tokamak Energy oEmbed API
  slug: tokamak-energy-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/openapi/tokamak-energy-oembed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Tokamak Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tokamak Energy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tokamak Energy
provider_slug: tokamak-energy
scheme_count: 1
schemes:
- description: WordPress Application Passwords (HTTP Basic). Declared by this site at GET /wp-json/ under authentication.application-passwords. Required only for authenticated scopes and write operations; every operation described in this document is readable anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/tokamak-energy-area-items-api-openapi.yml
  - openapi/tokamak-energy-authors-api-openapi.yml
  - openapi/tokamak-energy-discovery-api-openapi.yml
  - openapi/tokamak-energy-media-api-openapi.yml
  - openapi/tokamak-energy-oembed-api-openapi.yml
  - openapi/tokamak-energy-pages-api-openapi.yml
  - openapi/tokamak-energy-posts-api-openapi.yml
  - openapi/tokamak-energy-search-api-openapi.yml
  - openapi/tokamak-energy-taxonomy-api-openapi.yml
  type: http
slug: tokamak-energy-authentication
source_filename: tokamak-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://tokamakenergy.com/wp-json/ (authentication block, probed 2026-08-30) + the nine openapi/\n  documents in this repository\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (HTTP Basic). Declared by this site at GET /wp-json/ under\n    authentication.application-passwords. Required only for authenticated scopes and write operations;\n    every operation described in this document is readable anonymously.\n  sources:\n  - openapi/tokamak-energy-area-items-api-openapi.yml\n  - openapi/tokamak-energy-authors-api-openapi.yml\n  - openapi/tokamak-energy-discovery-api-openapi.yml\n  - openapi/tokamak-energy-media-api-openapi.yml\n  - openapi/tokamak-energy-oembed-api-openapi.yml\n  - openapi/tokamak-energy-pages-api-openapi.yml\n  - openapi/tokamak-energy-posts-api-openapi.yml\n  - openapi/tokamak-energy-search-api-openapi.yml\n\
  \  - openapi/tokamak-energy-taxonomy-api-openapi.yml\nanonymous_access:\n  supported: true\n  note: Every operation profiled in this repository returns HTTP 200 to an unauthenticated GET. Verified\n    live 2026-08-30 against posts, pages, media, area-item, categories, tags, users, search, types, taxonomies\n    and oembed.\n  verified: '2026-08-30'\nauthenticated_scopes:\n  mechanism: WordPress Application Passwords (HTTP Basic)\n  authorization_endpoint: https://tokamakenergy.com/wp-admin/authorize-application.php\n  declared_at: https://tokamakenergy.com/wp-json/ -> authentication.application-passwords.endpoints.authorization\n  note: 'This is the only authentication method this host advertises. It is an operator credential for\n    site editors, not a developer-programme credential: Tokamak Energy issues no API keys and runs no\n    signup for API access. Write operations (POST/PUT/PATCH/DELETE on posts, pages, media, area-item,\n    taxonomy terms, users, settings) and the edit context\
  \ require it.'\nobserved:\n- request: GET https://tokamakenergy.com/wp-json/wp/v2/posts?per_page=1\n  status: 200\n  auth: none\n- request: GET https://tokamakenergy.com/wp-json/wp/v2/settings\n  status: 401\n  auth: none\n  body_code: rest_forbidden\n- request: GET https://tokamakenergy.com/wp-json/wp/v2/comments\n  status: 403\n  auth: none\n- request: GET https://tokamakenergy.com/wp-json/wp-abilities/v1/abilities\n  status: 401\n  auth: none\n  body_code: rest_forbidden\nno_oauth:\n  value: true\n  note: No OAuth 2.0 or OpenID Connect surface. /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    both returned 404. No scopes/ artifact is emitted, because there is no scope surface to document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tokamak-energy/refs/heads/main/authentication/tokamak-energy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fusion Energy
- Energy
- Superconductors
- HTS Magnets
- Advanced Manufacturing
- Deep Tech
- Plasma Physics
- Scientific Computing
- Research and Development
- Content
- United Kingdom
---
