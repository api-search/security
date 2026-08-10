---
api_key_in: []
api_specs:
- filename: accelsius-content-api-openapi.yml
  format: yaml
  label: Accelsius Resources Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-content-api-openapi.yml
- filename: accelsius-news-api-openapi.yml
  format: yaml
  label: Accelsius News API
  slug: news
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-news-api-openapi.yml
- filename: accelsius-pages-api-openapi.yml
  format: yaml
  label: Accelsius Pages API
  slug: pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-pages-api-openapi.yml
- filename: accelsius-media-api-openapi.yml
  format: yaml
  label: Accelsius Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-media-api-openapi.yml
- filename: accelsius-search-api-openapi.yml
  format: yaml
  label: Accelsius Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-search-api-openapi.yml
- filename: accelsius-discovery-api-openapi.yml
  format: yaml
  label: Accelsius API Discovery
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-discovery-api-openapi.yml
- filename: accelsius-categories-api-openapi.yml
  format: yaml
  label: Accelsius Categories API
  slug: accelsius-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-categories-api-openapi.yml
- filename: accelsius-media-folders-api-openapi.yml
  format: yaml
  label: Accelsius Media Folders API
  slug: accelsius-media-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-media-folders-api-openapi.yml
- filename: accelsius-registry-api-openapi.yml
  format: yaml
  label: Accelsius Registry API
  slug: accelsius-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-registry-api-openapi.yml
- filename: accelsius-tags-api-openapi.yml
  format: yaml
  label: Accelsius Tags API
  slug: accelsius-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-tags-api-openapi.yml
auth_types:
- none
- http
- cookie
description: ''
kind: authentication
layout: security
method: derived
name: Accelsius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accelsius secures its APIs with none, http, and cookie across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Accelsius
provider_slug: accelsius
scheme_count: 3
schemes:
- description: Anonymous public read access to the WordPress content API — resource-library posts, the news custom post type, pages, media, categories, tags, HappyFiles media folders, site search, and the type/taxonomy/status registries.
  evidence: 'GET /wp-json/wp/v2/posts?per_page=1 returned HTTP 200 with post JSON, `X-WP-Total: 154` and `Allow: GET`; the same anonymous request pattern returned 200 on news (8), pages (30), media (903), categories (8), tags (5), happyfiles_category (19), search (192), navigation, types, taxonomies and statuses.'
  name: public-read
  type: none
- description: WordPress Application Passwords over HTTP Basic — the one credential the site itself advertises. It governs the write half of these routes and the administrative read routes. It belongs to a logged-in Accelsius site editor; there is no public issuance path.
  evidence: The root index at https://accelsius.com/wp-json/ returns an `authentication` object whose `application-passwords.endpoints.authorization` value is https://accelsius.com/wp-admin/authorize-application.php.
  in: header
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/accelsius-content-api-openapi.yml
  - openapi/accelsius-discovery-api-openapi.yml
  - openapi/accelsius-media-api-openapi.yml
  - openapi/accelsius-news-api-openapi.yml
  - openapi/accelsius-pages-api-openapi.yml
  - openapi/accelsius-search-api-openapi.yml
  - openapi/accelsius-taxonomy-api-openapi.yml
  type: http
- description: WordPress core cookie authentication paired with an X-WP-Nonce request header, the browser-side equivalent used by the site's own editor. Not a public developer credential.
  evidence: '`Access-Control-Allow-Headers` on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`.'
  in: cookie
  name: wordpress-cookie-nonce
  type: cookie
slug: accelsius-authentication
source_filename: accelsius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: >-\n  live anonymous probes of https://accelsius.com/wp-json/ (2026-08-06) plus this repo's\n  openapi/accelsius-*-openapi.yml\nsummary:\n  types:\n  - none\n  - http\n  - cookie\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Accelsius publishes no developer program and no product API. Its only machine-readable\n    surface is the platform-provided WordPress REST API at accelsius.com/wp-json/, and the read\n    half of that surface is fully public: every operation documented in this repo's openapi/\n    specs was verified to return HTTP 200 with JSON to an anonymous request carrying no\n    credentials of any kind. There is no API key, no OAuth, no OpenID Connect, no signup and no\n    developer credential to obtain — /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server both returned 404. Unlike a stock install, this root\n    index does advertise one scheme: `authentication.application-passwords`,\
  \ whose authorization\n    endpoint is https://accelsius.com/wp-admin/authorize-application.php. That is an\n    administrative WordPress credential for site editors, not a public developer credential, and\n    it exists to serve the write half of the same routes. Those write operations are deliberately\n    NOT documented in this repo's openapi/ specs, which describe only the anonymously reachable\n    read surface.\nschemes:\n- name: public-read\n  type: none\n  description: >-\n    Anonymous public read access to the WordPress content API — resource-library posts, the news\n    custom post type, pages, media, categories, tags, HappyFiles media folders, site search, and\n    the type/taxonomy/status registries.\n  evidence: >-\n    GET /wp-json/wp/v2/posts?per_page=1 returned HTTP 200 with post JSON, `X-WP-Total: 154` and\n    `Allow: GET`; the same anonymous request pattern returned 200 on news (8), pages (30),\n    media (903), categories (8), tags (5), happyfiles_category (19), search\
  \ (192), navigation,\n    types, taxonomies and statuses.\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords over HTTP Basic — the one credential the site itself\n    advertises. It governs the write half of these routes and the administrative read routes. It\n    belongs to a logged-in Accelsius site editor; there is no public issuance path.\n  in: header\n  evidence: >-\n    The root index at https://accelsius.com/wp-json/ returns an `authentication` object whose\n    `application-passwords.endpoints.authorization` value is\n    https://accelsius.com/wp-admin/authorize-application.php.\n  sources:\n  - openapi/accelsius-content-api-openapi.yml\n  - openapi/accelsius-discovery-api-openapi.yml\n  - openapi/accelsius-media-api-openapi.yml\n  - openapi/accelsius-news-api-openapi.yml\n  - openapi/accelsius-pages-api-openapi.yml\n  - openapi/accelsius-search-api-openapi.yml\n  - openapi/accelsius-taxonomy-api-openapi.yml\n- name:\
  \ wordpress-cookie-nonce\n  type: cookie\n  description: >-\n    WordPress core cookie authentication paired with an X-WP-Nonce request header, the\n    browser-side equivalent used by the site's own editor. Not a public developer credential.\n  in: cookie\n  evidence: >-\n    `Access-Control-Allow-Headers` on /wp-json/wp/v2/posts advertises `Authorization, X-WP-Nonce,\n    Content-Disposition, Content-MD5, Content-Type`.\ngated_surface:\n  description: >-\n    Routes present in the live route table but NOT anonymously readable. Recorded so the\n    public/private split of this surface is explicit rather than inferred. Every status below was\n    observed on 2026-08-06; the JSON error bodies behind them were not captured, because the\n    site's MalCare firewall began answering 403 to this pass before the bodies could be read (see\n    errors/accelsius-problem-types.yml).\n  routes:\n  - path: /wp/v2/settings\n    status: 401\n  - path: /wp/v2/menus\n    status: 401\n  - path: /wp/v2/menu-items\n\
  \    status: 401\n  - path: /wp/v2/menu-locations\n    status: 401\n  - path: /wp/v2/templates\n    status: 401\n  - path: /wp/v2/template-parts\n    status: 401\n  - path: /wp/v2/themes\n    status: 401\n  - path: /wp/v2/plugins\n    status: 401\n  - path: /wp/v2/widgets\n    status: 401\n  - path: /wp/v2/widget-types\n    status: 401\n  - path: /wp/v2/sidebars\n    status: 401\n  - path: /wp/v2/block-types\n    status: 401\n  - path: /wp/v2/block-patterns/patterns\n    status: 401\n  - path: /wp/v2/pattern-directory/patterns\n    status: 401\n  - path: /wp/v2/users/me\n    status: 401\n  - path: /wp-abilities/v1/abilities\n    status: 401\n  - path: /yoast/v1/statistics\n    status: 401\n  - path: /redirection/v1/redirect\n    status: 401\n  - path: /leadin/v1/access-token\n    status: 401\n  - path: /wp-site-health/v1/directory-sizes\n    status: 401\nexposed_personal_data:\n  route: /wp/v2/users\n  status: 200\n  count: 14\n  detail: >-\n    Unlike most of the administrative surface,\
  \ the WordPress user directory on this host answers\n    anonymously with HTTP 200 and 14 records. These are the site's content-author accounts — the\n    standard WordPress `view` context returns display name, slug, description, avatar URLs and\n    author-archive link, and no email address or password material. It is nonetheless a directory\n    of named individuals.\n  disposition: >-\n    Recorded here as an observed exposure and deliberately NOT modelled: no operation for\n    /wp/v2/users appears in this repo's openapi/ specs, no candidate MCP tool binds to it, and no\n    agent skill walks it. See the exclusion recorded in skills/_index.yml.\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nx-evidence:\n  fetched: '2026-08-06'\n  host: https://accelsius.com\n  root_index: https://accelsius.com/wp-json/\n  namespaces: 16\n  routes_advertised: 387\n  authentication_field:\n  - application-passwords\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/authentication/accelsius-authentication.yml
summary_line: none/http/cookie · 3 schemes
tags:
- Company
- Data Centers
- Liquid Cooling
- Thermal Management
- Direct-to-Chip Cooling
- Two-Phase Cooling
- Artificial Intelligence Infrastructure
- High Performance Computing
- Hardware
- Manufacturing
- Content
- WordPress
---
