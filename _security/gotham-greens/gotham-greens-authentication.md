---
api_key_in: []
api_specs:
- filename: gotham-greens-posts-api-openapi.yml
  format: yaml
  label: Gotham Greens Journal Posts API
  slug: gotham-greens-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-posts-api-openapi.yml
- filename: gotham-greens-pages-api-openapi.yml
  format: yaml
  label: Gotham Greens Pages API
  slug: gotham-greens-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-pages-api-openapi.yml
- filename: gotham-greens-media-api-openapi.yml
  format: yaml
  label: Gotham Greens Media API
  slug: gotham-greens-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-media-api-openapi.yml
- filename: gotham-greens-taxonomy-api-openapi.yml
  format: yaml
  label: Gotham Greens Taxonomy API
  slug: gotham-greens-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-taxonomy-api-openapi.yml
- filename: gotham-greens-search-api-openapi.yml
  format: yaml
  label: Gotham Greens Search API
  slug: gotham-greens-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-search-api-openapi.yml
- filename: gotham-greens-discovery-api-openapi.yml
  format: yaml
  label: Gotham Greens Discovery API
  slug: gotham-greens-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-discovery-api-openapi.yml
- filename: gotham-greens-oembed-api-openapi.yml
  format: yaml
  label: Gotham Greens oEmbed API
  slug: gotham-greens-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-oembed-api-openapi.yml
- filename: gotham-greens-seo-api-openapi.yml
  format: yaml
  label: Gotham Greens SEO Metadata API
  slug: gotham-greens-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/openapi/gotham-greens-seo-api-openapi.yml
auth_types:
- none
- cookie
description: ''
kind: authentication
layout: security
method: derived
name: Gotham Greens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gotham Greens secures its APIs with none and cookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gotham Greens
provider_slug: gotham-greens
scheme_count: 2
schemes:
- description: Anonymous public read access to the WordPress content API — posts, pages, media, categories, tags, search, oEmbed, the Yoast SEO head endpoint, and the type/taxonomy/status registries.
  evidence: 'GET /wp-json/wp/v2/posts?per_page=1 returned 200 with post JSON and X-WP-Total: 132; the same anonymous request pattern returned 200 on pages, media, categories, tags, comments, search, types, taxonomies, statuses, oembed/1.0/embed and yoast/v1/get_head.'
  name: public-read
  type: none
- description: WordPress core cookie authentication paired with an X-WP-Nonce request header, required for the write half of the same routes and for the administrative read routes. Not a public developer credential — it belongs to a logged-in site user.
  evidence: 'Access-Control-Allow-Headers on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`. Anonymous GETs against the administrative routes returned 401: /wp/v2/users (rest_user_cannot_view), /wp/v2/settings (rest_forbidden), /wp/v2/themes (rest_cannot_view_themes), /wp/v2/plugins (rest_cannot_view_plugins), /wp/v2/menus (rest_cannot_view), /wp/v2/block-types (rest_block_type_cannot_view) and /wp/v2/posts/{id}/revisions (rest_cannot_read).'
  in: cookie
  name: wordpress-cookie-nonce
  type: cookie
slug: gotham-greens-authentication
source_filename: gotham-greens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: live anonymous probes of https://www.gothamgreens.com/wp-json/ (2026-08-01)\nsummary:\n  types:\n  - none\n  - cookie\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Gotham Greens publishes no developer program and no product API. Its only machine-readable\n    surface is the platform-provided WordPress REST API at /wp-json/, and the read half of that\n    surface is fully public: every operation documented in this repo's openapi/ specs was\n    verified to return HTTP 200 with JSON to an anonymous request carrying no credentials of any\n    kind. There is no API key, no OAuth, no signup, and no rate-limit or quota signalling\n    observed. The root index advertises an EMPTY `authentication` array — the site registers no\n    additional REST authentication scheme beyond WordPress core. Write operations (POST/PUT/\n    PATCH/DELETE) are registered on the same routes but reject anonymous callers with HTTP 401;\n    they\
  \ require a logged-in WordPress session cookie plus an X-WP-Nonce header, or an\n    Application Password over HTTP Basic — both administrative credentials, not a public\n    developer credential. Those write operations are deliberately NOT documented in the openapi/\n    specs, which describe only the anonymously reachable read surface.\nschemes:\n- name: public-read\n  type: none\n  description: >-\n    Anonymous public read access to the WordPress content API — posts, pages, media, categories,\n    tags, search, oEmbed, the Yoast SEO head endpoint, and the type/taxonomy/status registries.\n  evidence: >-\n    GET /wp-json/wp/v2/posts?per_page=1 returned 200 with post JSON and X-WP-Total: 132; the same\n    anonymous request pattern returned 200 on pages, media, categories, tags, comments, search,\n    types, taxonomies, statuses, oembed/1.0/embed and yoast/v1/get_head.\n- name: wordpress-cookie-nonce\n  type: cookie\n  description: >-\n    WordPress core cookie authentication paired\
  \ with an X-WP-Nonce request header, required for\n    the write half of the same routes and for the administrative read routes. Not a public\n    developer credential — it belongs to a logged-in site user.\n  in: cookie\n  evidence: >-\n    Access-Control-Allow-Headers on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce,\n    Content-Disposition, Content-MD5, Content-Type`. Anonymous GETs against the administrative\n    routes returned 401: /wp/v2/users (rest_user_cannot_view), /wp/v2/settings (rest_forbidden),\n    /wp/v2/themes (rest_cannot_view_themes), /wp/v2/plugins (rest_cannot_view_plugins),\n    /wp/v2/menus (rest_cannot_view), /wp/v2/block-types (rest_block_type_cannot_view) and\n    /wp/v2/posts/{id}/revisions (rest_cannot_read).\ngated_surface:\n  description: >-\n    Routes present in the live route table but not anonymously readable. Recorded so the public\n    /private split of this surface is explicit rather than inferred.\n  routes:\n  - path: /wp/v2/users\n\
  \    status: 401\n    code: rest_user_cannot_view\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/posts/{id}/revisions\n    status: 401\n    code: rest_cannot_read\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nx-evidence:\n  fetched: '2026-08-01'\n  host: https://www.gothamgreens.com\n  root_index: https://www.gothamgreens.com/wp-json/\n  namespaces: 17\n  routes_advertised: 406\n  authentication_field: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/authentication/gotham-greens-authentication.yml
summary_line: none/cookie · 2 schemes
tags:
- Company
- Agriculture
- Controlled Environment Agriculture
- Hydroponics
- Food
- Consumer Packaged Goods
- Fresh Produce
- Sustainability
- Urban Farming
- Content
---
