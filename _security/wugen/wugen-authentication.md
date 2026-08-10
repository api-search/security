---
api_key_in: []
api_specs:
- filename: wugen-comments-api-openapi.yml
  format: yaml
  label: Wugen Comments API
  slug: wugen-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-comments-api-openapi.yml
- filename: wugen-discovery-api-openapi.yml
  format: yaml
  label: Wugen Discovery API
  slug: wugen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-discovery-api-openapi.yml
- filename: wugen-media-api-openapi.yml
  format: yaml
  label: Wugen Media API
  slug: wugen-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-media-api-openapi.yml
- filename: wugen-pages-api-openapi.yml
  format: yaml
  label: Wugen Pages API
  slug: wugen-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-pages-api-openapi.yml
- filename: wugen-posts-api-openapi.yml
  format: yaml
  label: Wugen Posts API
  slug: wugen-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-posts-api-openapi.yml
- filename: wugen-search-api-openapi.yml
  format: yaml
  label: Wugen Search API
  slug: wugen-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-search-api-openapi.yml
- filename: wugen-taxonomy-api-openapi.yml
  format: yaml
  label: Wugen Taxonomy API
  slug: wugen-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Wugen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wugen declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Wugen
provider_slug: wugen
scheme_count: 0
schemes: []
slug: wugen-authentication
source_filename: wugen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live anonymous probes of https://alloteratx.com/wp-json and https://wugen.com/wp-json\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\n  note: >-\n    Neither the derived OpenAPI nor the live route-discovery documents declare any security scheme,\n    because the read surface catalogued in this repo requires none. The entire wp/v2 content read\n    surface on both hosts — posts, pages, media, categories, tags, comments, search and the\n    type/taxonomy/status discovery documents — is served anonymously over HTTPS with no credential\n    of any kind. `derive-authentication.py` therefore produced no schemes for this provider; that is\n    a true result, not a gap.\nmodel: no-auth-read / gated-write\nposture: >-\n  Allotera runs stock WordPress core authentication. There is no developer program, no API key\n \
  \ issuance, no OAuth authorization server (/.well-known/oauth-authorization-server returns 404 on\n  alloteratx.com and a soft 404 on wugen.com), and no published authentication documentation of the\n  company's own. Write access and the privileged read routes fall back to WordPress's built-in\n  mechanisms — cookie authentication plus an X-WP-Nonce header for same-origin browser sessions, and\n  HTTP Basic with an Application Password for external clients — neither of which is available to a\n  third party without an account on the site.\nobserved:\n  anonymous_read_allowed:\n  - route: /wp/v2/posts\n    status: 200\n  - route: /wp/v2/pages\n    status: 200\n  - route: /wp/v2/media\n    status: 200\n  - route: /wp/v2/categories\n    status: 200\n  - route: /wp/v2/tags\n    status: 200\n  - route: /wp/v2/comments\n    status: 200\n  - route: /wp/v2/search\n    status: 200\n  - route: /wp/v2/types\n    status: 200\n  - route: /wp/v2/taxonomies\n    status: 200\n  - route: /wp/v2/statuses\n\
  \    status: 200\n  authentication_required:\n  - route: /wp/v2/users\n    status: 401\n    code: rest_user_cannot_view\n    message: Sorry, you are not allowed to list users.\n  - route: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - route: /wp/v2/themes\n    status: 401\n    code: rest_forbidden\n  - route: /wp/v2/plugins\n    status: 401\n    code: rest_forbidden\n  - route: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    host: alloteratx.com\n    note: >-\n      The WordPress Abilities API namespace is registered on alloteratx.com but its registry is\n      authentication-gated, so the ability set could not be enumerated anonymously. There is no MCP\n      namespace on either host.\n  cors:\n    access_control_allow_headers:\n    - Authorization\n    - X-WP-Nonce\n    - Content-Disposition\n    - Content-MD5\n    - Content-Type\n    access_control_expose_headers:\n    - X-WP-Total\n    - X-WP-TotalPages\n    - Link\n    note: >-\n      The\
  \ Authorization and X-WP-Nonce entries in Access-Control-Allow-Headers are WordPress core\n      defaults advertising the two supported credential mechanisms; they are not evidence of a\n      credential a third party can obtain.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/authentication/wugen-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- CAR-T
- CRISPR
- Immunotherapy
- Research
- Content
---
