---
api_key_in: []
api_specs:
- filename: burger-singh-pages-api-openapi.yml
  format: yaml
  label: Burger Singh Pages API
  slug: burger-singh-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-pages-api-openapi.yml
- filename: burger-singh-media-api-openapi.yml
  format: yaml
  label: Burger Singh Media API
  slug: burger-singh-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-media-api-openapi.yml
- filename: burger-singh-taxonomy-api-openapi.yml
  format: yaml
  label: Burger Singh Taxonomy API
  slug: burger-singh-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-taxonomy-api-openapi.yml
- filename: burger-singh-search-api-openapi.yml
  format: yaml
  label: Burger Singh Search API
  slug: burger-singh-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-search-api-openapi.yml
- filename: burger-singh-discovery-api-openapi.yml
  format: yaml
  label: Burger Singh Discovery API
  slug: burger-singh-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-discovery-api-openapi.yml
- filename: burger-singh-seo-api-openapi.yml
  format: yaml
  label: Burger Singh SEO Metadata API
  slug: burger-singh-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-seo-api-openapi.yml
auth_types:
- none
- cookie
- http-basic
description: ''
kind: authentication
layout: security
method: probed
name: Burger Singh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Burger Singh secures its APIs with none, cookie, and http-basic across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Burger Singh
provider_slug: burger-singh
scheme_count: 3
schemes:
- description: Anonymous public read access to the WordPress content API - pages, media, categories, tags, search, public authors, the Yoast SEO head endpoint, and the type/taxonomy/status registries.
  evidence: 'GET /wp-json/wp/v2/pages?per_page=1 returned 200 with page JSON and X-WP-Total: 20; the same anonymous request pattern returned 200 on media (X-WP-Total: 576), categories (13), tags (0), comments (0), search, users (1), types, taxonomies, statuses and yoast/v1/get_head.'
  name: public-read
  type: none
- description: WordPress core cookie authentication paired with an X-WP-Nonce request header, required for the write half of the same routes and for the administrative read routes. Not a public developer credential - it belongs to a logged-in site user.
  evidence: Access-Control-Allow-Headers on /wp-json/wp/v2/pages advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`. Anonymous GETs against the administrative routes returned 401 (see gated_surface below).
  in: cookie
  name: wordpress-cookie-nonce
  type: cookie
- authorization_endpoint: https://www.burgersinghonline.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords over HTTP Basic, declared in the root index `authentication` object. Issued interactively to an existing WordPress user at the authorization endpoint below; there is no public registration or self-serve issuance.
  evidence: The live root index at /wp-json/ returns {"authentication":{"application-passwords":{"endpoints":{"authorization":"https://www.burgersinghonline.com/wp-admin/authorize-application.php"}}}}.
  name: application-passwords
  scheme: basic
  type: http
slug: burger-singh-authentication
source_filename: burger-singh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live anonymous probes of https://www.burgersinghonline.com/wp-json/ (2026-08-08)\nsummary:\n  types:\n  - none\n  - cookie\n  - http-basic\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Burger Singh publishes no developer program and no product API. Its only machine-readable\n    surface is the platform-provided WordPress REST API at /wp-json/ behind burgersinghonline.com,\n    and the read half of that surface is fully public: every operation documented in this repo's\n    openapi/ specs was verified to return HTTP 200 with JSON to an anonymous request carrying no\n    credentials of any kind. There is no API key, no OAuth, no signup, and no rate-limit or quota\n    signalling was observed. Unlike a default WordPress install the root index does advertise one\n    authentication method - `application-passwords`, with its authorization endpoint at\n    /wp-admin/authorize-application.php - but that is an administrative\
  \ site credential issued to a\n    logged-in WordPress user, not a public developer credential, and there is no self-serve path to\n    obtain one. Write operations (POST/PUT/PATCH/DELETE) are registered on the same routes but\n    reject anonymous callers; they require a logged-in WordPress session cookie plus an X-WP-Nonce\n    header, or an Application Password over HTTP Basic. Those write operations are deliberately NOT\n    documented in the openapi/ specs, which describe only the anonymously reachable read surface.\nschemes:\n- name: public-read\n  type: none\n  description: >-\n    Anonymous public read access to the WordPress content API - pages, media, categories, tags,\n    search, public authors, the Yoast SEO head endpoint, and the type/taxonomy/status registries.\n  evidence: >-\n    GET /wp-json/wp/v2/pages?per_page=1 returned 200 with page JSON and X-WP-Total: 20; the same\n    anonymous request pattern returned 200 on media (X-WP-Total: 576), categories (13), tags (0),\n\
  \    comments (0), search, users (1), types, taxonomies, statuses and yoast/v1/get_head.\n- name: wordpress-cookie-nonce\n  type: cookie\n  in: cookie\n  description: >-\n    WordPress core cookie authentication paired with an X-WP-Nonce request header, required for the\n    write half of the same routes and for the administrative read routes. Not a public developer\n    credential - it belongs to a logged-in site user.\n  evidence: >-\n    Access-Control-Allow-Headers on /wp-json/wp/v2/pages advertises `Authorization, X-WP-Nonce,\n    Content-Disposition, Content-MD5, Content-Type`. Anonymous GETs against the administrative\n    routes returned 401 (see gated_surface below).\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords over HTTP Basic, declared in the root index `authentication`\n    object. Issued interactively to an existing WordPress user at the authorization endpoint below;\n    there is no public registration\
  \ or self-serve issuance.\n  authorization_endpoint: https://www.burgersinghonline.com/wp-admin/authorize-application.php\n  evidence: >-\n    The live root index at /wp-json/ returns\n    {\"authentication\":{\"application-passwords\":{\"endpoints\":{\"authorization\":\"https://www.burgersinghonline.com/wp-admin/authorize-application.php\"}}}}.\ngated_surface:\n  description: >-\n    Routes present in the live route table but not anonymously readable. Recorded so the\n    public/private split of this surface is explicit rather than inferred. Every status and code\n    below was observed on 2026-08-08.\n  routes:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n\
  \  - path: /wp/v2/templates\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/pages/{id}/revisions\n    status: 401\n    code: rest_cannot_read\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities API - the agent-facing capability registry - is registered on this\n      host but is entirely credentialed. No ability names, descriptions or input schemas are\n      readable anonymously, so none are recorded in this repo.\n  - path: /wp-site-health/v1/tests/https-status\n    status: 401\n    code: rest_forbidden\n  - path: /psd/v1/get-logs\n    status: 401\n    code: rest_forbidden\n  - path: /contact-form-7/v1/contact-forms\n    status: 403\n    code: wpcf7_forbidden\n  - path: /post-smtp/v1/get-logs\n    status: 400\n    code: 'Auth token missing.'\n    note: >-\n      Plugin route with a non-WordPress error envelope - returns\n      {\"success\":false,\"data\":{\"error\":\"Auth token missing.\"\
  }} rather than the core code/message/data\n      shape.\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nx-evidence:\n  fetched: '2026-08-08'\n  host: https://www.burgersinghonline.com\n  root_index: https://www.burgersinghonline.com/wp-json/\n  http_status: 200\n  namespaces: 12\n  routes_advertised: 200\n  authentication_field:\n  - application-passwords\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/authentication/burger-singh-authentication.yml
summary_line: none/cookie/http-basic · 3 schemes
tags:
- Company
- Restaurant
- Quick Service Restaurant
- Food and Beverage
- Franchising
- Consumer
- India
- Retail
- Content
- WordPress
---
