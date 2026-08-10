---
api_key_in: []
api_specs:
- filename: cresilon-posts-api-openapi.yml
  format: yaml
  label: Cresilon News & Press Releases API
  slug: cresilon-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-posts-api-openapi.yml
- filename: cresilon-pages-api-openapi.yml
  format: yaml
  label: Cresilon Pages API
  slug: cresilon-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-pages-api-openapi.yml
- filename: cresilon-media-api-openapi.yml
  format: yaml
  label: Cresilon Media API
  slug: cresilon-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-media-api-openapi.yml
- filename: cresilon-taxonomy-api-openapi.yml
  format: yaml
  label: Cresilon Taxonomy API
  slug: cresilon-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-taxonomy-api-openapi.yml
- filename: cresilon-search-api-openapi.yml
  format: yaml
  label: Cresilon Search API
  slug: cresilon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-search-api-openapi.yml
- filename: cresilon-discovery-api-openapi.yml
  format: yaml
  label: Cresilon Discovery API
  slug: cresilon-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-discovery-api-openapi.yml
- filename: cresilon-oembed-api-openapi.yml
  format: yaml
  label: Cresilon oEmbed API
  slug: cresilon-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-oembed-api-openapi.yml
- filename: cresilon-seo-api-openapi.yml
  format: yaml
  label: Cresilon SEO Metadata API
  slug: cresilon-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-seo-api-openapi.yml
- filename: cresilon-authors-api-openapi.yml
  format: yaml
  label: Cresilon Authors API
  slug: cresilon-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-authors-api-openapi.yml
- filename: cresilon-comments-api-openapi.yml
  format: yaml
  label: Cresilon Comments API
  slug: cresilon-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-comments-api-openapi.yml
auth_types:
- none
- cookie
- basic
description: ''
kind: authentication
layout: security
method: derived
name: Cresilon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cresilon secures its APIs with none, cookie, and basic across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cresilon
provider_slug: cresilon
scheme_count: 3
schemes:
- description: Anonymous public read access to the WordPress content API — posts, pages, media, categories, tags, comments, authors, search, oEmbed, the Yoast SEO head endpoint, and the type/taxonomy/status registries.
  evidence: 'GET /wp-json/wp/v2/posts?per_page=1 returned 200 with post JSON and X-WP-Total: 36; the same anonymous request pattern returned 200 on pages (53), media (1307), categories (2), tags (4), users (1), comments (0), search, types, taxonomies, statuses, oembed/1.0/embed and yoast/v1/get_head.'
  name: public-read
  type: none
- description: WordPress core cookie authentication paired with an X-WP-Nonce request header, required for the write half of the same routes and for the administrative read routes. Not a public developer credential — it belongs to a logged-in site user.
  evidence: Access-Control-Allow-Headers on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`.
  in: cookie
  name: wordpress-cookie-nonce
  type: cookie
- authorization_endpoint: https://cresilon.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords over HTTP Basic. This is the ONLY authentication method the site advertises in its REST root index, and it is an administrative credential issued to an existing WordPress user — there is no self-service developer signup behind it.
  evidence: 'The root index at https://cresilon.com/wp-json/ returns `"authentication": {"application-passwords": {"endpoints": {"authorization": "https://cresilon.com/wp-admin/authorize-application.php"}}}`.'
  name: application-passwords
  public_credential: false
  scheme: basic
  type: http
slug: cresilon-authentication
source_filename: cresilon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: live anonymous probes of https://cresilon.com/wp-json/ (2026-08-04)\nsummary:\n  types:\n  - none\n  - cookie\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Cresilon is a biotechnology and medical-device manufacturer. It publishes no developer\n    program, no API documentation and no product API. Its only machine-readable surface is the\n    platform-provided WordPress REST API at /wp-json/, and the read half of that surface is fully\n    public: every operation documented in this repo's openapi/ specs was verified to return HTTP\n    200 with JSON to an anonymous request carrying no credentials of any kind. There is no API\n    key, no OAuth, no developer signup, and no rate-limit or quota signalling observed. Unlike\n    most WordPress deployments in this catalog, the root index DOES advertise an authentication\n    method — WordPress Application Passwords, with an authorization endpoint at\n    https://cresilon.com/wp-admin/authorize-application.php.\
  \ That is an administrative credential\n    for a site user, not a public developer credential, and the pipeline did not and will not\n    attempt to obtain one. Write operations (POST/PUT/PATCH/DELETE) are registered on the same\n    routes but reject anonymous callers with HTTP 401; they require a logged-in WordPress session\n    cookie plus an X-WP-Nonce header, or an Application Password over HTTP Basic. Those write\n    operations are deliberately NOT documented in the openapi/ specs, which describe only the\n    anonymously reachable read surface.\nschemes:\n- name: public-read\n  type: none\n  description: >-\n    Anonymous public read access to the WordPress content API — posts, pages, media, categories,\n    tags, comments, authors, search, oEmbed, the Yoast SEO head endpoint, and the\n    type/taxonomy/status registries.\n  evidence: >-\n    GET /wp-json/wp/v2/posts?per_page=1 returned 200 with post JSON and X-WP-Total: 36; the same\n    anonymous request pattern returned 200\
  \ on pages (53), media (1307), categories (2), tags (4),\n    users (1), comments (0), search, types, taxonomies, statuses, oembed/1.0/embed and\n    yoast/v1/get_head.\n- name: wordpress-cookie-nonce\n  type: cookie\n  in: cookie\n  description: >-\n    WordPress core cookie authentication paired with an X-WP-Nonce request header, required for\n    the write half of the same routes and for the administrative read routes. Not a public\n    developer credential — it belongs to a logged-in site user.\n  evidence: >-\n    Access-Control-Allow-Headers on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce,\n    Content-Disposition, Content-MD5, Content-Type`.\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords over HTTP Basic. This is the ONLY authentication method the\n    site advertises in its REST root index, and it is an administrative credential issued to an\n    existing WordPress user — there is no self-service\
  \ developer signup behind it.\n  authorization_endpoint: https://cresilon.com/wp-admin/authorize-application.php\n  evidence: >-\n    The root index at https://cresilon.com/wp-json/ returns\n    `\"authentication\": {\"application-passwords\": {\"endpoints\": {\"authorization\":\n    \"https://cresilon.com/wp-admin/authorize-application.php\"}}}`.\n  public_credential: false\nsite_member_area:\n  description: >-\n    Separate from the REST surface, cresilon.com runs a human-facing member area (WordPress\n    Download Manager) gating TRAUMAGEL and VETIGEL resource downloads. It is a web login, not an\n    API credential, and no REST route exposes it anonymously.\n  register: https://cresilon.com/register/\n  login: https://cresilon.com/login/\n  account: https://cresilon.com/account/\n  distributor_portal:\n    url: https://cresilon.com/distributor-portal/\n    gate: WordPress page password (verified live — the page renders a single password prompt)\n  evidence: >-\n    GET /register/ returned\
  \ 200 with a real registration form (10 inputs); GET /login/ returned\n    200 with a real login form; GET /distributor-portal/ returned 200 with \"This content is\n    password-protected.\"\ngated_surface:\n  description: >-\n    Routes present in the live route table but NOT anonymously readable. Recorded so the\n    public/private split of this surface is explicit rather than inferred.\n  routes:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/menu-items\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/templates\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/template-parts\n    status: 401\n    code:\
  \ rest_cannot_manage_templates\n  - path: /wp/v2/pattern-directory/patterns\n    status: 401\n    code: rest_pattern_directory_cannot_view\n  - path: /wp/v2/font-families\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/posts/{id}/revisions\n    status: 401\n    code: rest_cannot_read\n  - path: /oembed/1.0/proxy\n    status: 401\n    code: rest_forbidden\n  - path: /jetpack/v4/site\n    status: 401\n    code: invalid_user_permission_view_admin\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n  - path: /wp-site-health/v1/tests/background-updates\n    status: 401\nnotable_difference_from_catalog_norm: >-\n  On most WordPress sites in this catalog /wp/v2/users returns 401 (rest_user_cannot_view). On\n  cresilon.com it returns 200 with a single author record (id 211412379, slug `cresilon`), so the\n  numeric `author` field on every post IS publicly resolvable here.\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\n\
  x-evidence:\n  fetched: '2026-08-04'\n  host: https://cresilon.com\n  root_index: https://cresilon.com/wp-json/\n  namespaces: 45\n  routes_advertised: 1021\n  authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://cresilon.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/authentication/cresilon-authentication.yml
summary_line: none/cookie/basic · 3 schemes
tags:
- Company
- Biotechnology
- Medical Devices
- Health
- Hemostasis
- Wound Care
- Trauma Care
- Veterinary
- Life Sciences
- Manufacturing
- Content
---
