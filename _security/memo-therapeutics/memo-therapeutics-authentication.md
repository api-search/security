---
api_key_in: []
api_specs:
- filename: memo-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Posts API
  slug: memo-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-posts-api-openapi.yml
- filename: memo-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Pages API
  slug: memo-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-pages-api-openapi.yml
- filename: memo-therapeutics-media-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Media API
  slug: memo-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-media-api-openapi.yml
- filename: memo-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Taxonomy API
  slug: memo-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-taxonomy-api-openapi.yml
- filename: memo-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Comments API
  slug: memo-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-comments-api-openapi.yml
- filename: memo-therapeutics-search-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Search API
  slug: memo-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-search-api-openapi.yml
- filename: memo-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Discovery API
  slug: memo-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-discovery-api-openapi.yml
- filename: memo-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Memo Therapeutics oEmbed API
  slug: memo-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-oembed-api-openapi.yml
- filename: memo-therapeutics-navigation-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Navigation API
  slug: memo-therapeutics-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-navigation-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Memo Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memo Therapeutics declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Memo Therapeutics
provider_slug: memo-therapeutics
scheme_count: 3
schemes:
- applies_to: read
  description: Anonymous GET. Confirmed on /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/comments, /wp/v2/categories, /wp/v2/tags, /wp/v2/search, /wp/v2/navigation, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses and /oembed/1.0/embed, all HTTP 200 on 2026-08-25.
  id: none
  type: none
- applies_to: write
  description: 'WordPress core''s first-party scheme — a logged-in session cookie plus an X-WP-Nonce header. Advertised by the deployment: the response to an anonymous call carries "access-control-allow-headers: Authorization, X-WP-Nonce, ...". Not obtainable by an outside integrator; it exists for the site''s own editor UI.'
  id: cookie-nonce
  status: gated
  type: cookie
- applies_to: write
  description: An Authorization header is accepted by the origin (wp-site-health/v1/tests/authorization-header is registered), which is how WordPress Application Passwords would be presented. No credential is issued to third parties, so this is a capability of the software, not an access model Memo Therapeutics operates.
  id: authorization-header
  status: gated
  type: http
slug: memo-therapeutics-authentication
source_filename: memo-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://memo-therapeutics.com/wp-json on 2026-08-25, plus the route\n  index the site publishes at /wp-json/. Memo Therapeutics publishes no authentication\n  documentation of its own; the upstream contract is defined at\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary: >-\n  The published read surface requires no credentials at all. Every write operation and every\n  administrative namespace is closed to anonymous clients and answers 401 with the WordPress REST\n  error envelope. There is no API key programme, no OAuth server, no token endpoint and no\n  developer sign-up — Memo Therapeutics does not issue credentials for this surface to anyone\n  outside the company.\nschemes:\n- id: none\n  type: none\n  description: >-\n    Anonymous GET. Confirmed on /wp/v2/posts, /wp/v2/pages,\
  \ /wp/v2/media, /wp/v2/comments,\n    /wp/v2/categories, /wp/v2/tags, /wp/v2/search, /wp/v2/navigation, /wp/v2/types,\n    /wp/v2/taxonomies, /wp/v2/statuses and /oembed/1.0/embed, all HTTP 200 on 2026-08-25.\n  applies_to: read\n- id: cookie-nonce\n  type: cookie\n  description: >-\n    WordPress core's first-party scheme — a logged-in session cookie plus an X-WP-Nonce header.\n    Advertised by the deployment: the response to an anonymous call carries\n    \"access-control-allow-headers: Authorization, X-WP-Nonce, ...\". Not obtainable by an outside\n    integrator; it exists for the site's own editor UI.\n  applies_to: write\n  status: gated\n- id: authorization-header\n  type: http\n  description: >-\n    An Authorization header is accepted by the origin (wp-site-health/v1/tests/authorization-header\n    is registered), which is how WordPress Application Passwords would be presented. No credential\n    is issued to third parties, so this is a capability of the software, not an access\
  \ model\n    Memo Therapeutics operates.\n  applies_to: write\n  status: gated\ngated_surface:\n  observed_status: 401\n  error_codes:\n  - rest_forbidden\n  - rest_user_cannot_view\n  - rest_cannot_view\n  - rest_cannot_view_themes\n  - rest_cannot_view_plugins\n  - rest_block_type_cannot_view\n  - rest_cannot_read\n  paths:\n  - /wp/v2/users\n  - /wp/v2/settings\n  - /wp/v2/menus\n  - /wp/v2/themes\n  - /wp/v2/plugins\n  - /wp/v2/block-types\n  - /wp/v2/font-collections\n  - /wp-abilities/v1/abilities\n  - /aioseo/v1/ping\n  - /aioseo/v1/ai-agents/mcp-adapter/release\n  note: >-\n    /wp-json/batch/v1 returned 403 from the edge (an HTML Apache error page), not the JSON 401 the\n    application returns — the WAF answers before WordPress does on that path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/authentication/memo-therapeutics-authentication.yml
summary_line: 3 schemes
tags:
- Company
- biotechnology
- pharmaceuticals
- antibody-therapeutics
- rare-disease
- nephrology
- transplantation
- virology
- oncology
- clinical-trials
- life-sciences
- switzerland
- content-api
---
