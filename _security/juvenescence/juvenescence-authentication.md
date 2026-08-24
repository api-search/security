---
api_key_in: []
api_specs:
- filename: juvenescence-posts-api-openapi.yml
  format: yaml
  label: Juvenescence Posts API
  slug: juvenescence-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-posts-api-openapi.yml
- filename: juvenescence-pages-api-openapi.yml
  format: yaml
  label: Juvenescence Pages API
  slug: juvenescence-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-pages-api-openapi.yml
- filename: juvenescence-media-api-openapi.yml
  format: yaml
  label: Juvenescence Media API
  slug: juvenescence-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-media-api-openapi.yml
- filename: juvenescence-categories-api-openapi.yml
  format: yaml
  label: Juvenescence Categories API
  slug: juvenescence-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-categories-api-openapi.yml
- filename: juvenescence-tags-api-openapi.yml
  format: yaml
  label: Juvenescence Tags API
  slug: juvenescence-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-tags-api-openapi.yml
- filename: juvenescence-comments-api-openapi.yml
  format: yaml
  label: Juvenescence Comments API
  slug: juvenescence-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-comments-api-openapi.yml
- filename: juvenescence-search-api-openapi.yml
  format: yaml
  label: Juvenescence Search API
  slug: juvenescence-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-search-api-openapi.yml
- filename: juvenescence-portfolio-api-openapi.yml
  format: yaml
  label: Juvenescence Portfolio API
  slug: juvenescence-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-portfolio-api-openapi.yml
- filename: juvenescence-discovery-api-openapi.yml
  format: yaml
  label: Juvenescence Discovery API
  slug: juvenescence-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-discovery-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Juvenescence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juvenescence declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Juvenescence
provider_slug: juvenescence
scheme_count: 0
schemes: []
slug: juvenescence-authentication
source_filename: juvenescence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  openapi/_original/juvenescence-content-openapi.yml, https://juvlabs.com/wp-json/ (site index), and\n  live anonymous GETs against every wp/v2 route on 2026-08-23\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary: >-\n  The Juvenescence content API requires NO credentials for everything this profile models. The site\n  index at https://juvlabs.com/wp-json/ returns \"authentication\": [] — the install advertises no\n  discoverable authentication scheme at all, no application-password endpoint discovery, no OAuth and\n  no OIDC. Anonymous callers get published posts, pages, media, taxonomy terms, search, the registered\n  content-type metadata and oEmbed. Administrative routes are registered on the same namespace but\n  reject anonymous callers with HTTP 401/403, and are not modelled as a public API surface. Because\n  there is no scope surface of any kind, no scopes/ artifact is emitted\
  \ for this provider.\nsecurity_schemes: []\npublic_access:\n  anonymous_read: true\n  api_key_required: false\n  registration_required: false\n  cors:\n    access_control_allow_headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type\n    access_control_expose_headers: X-WP-Total, X-WP-TotalPages, Link\n    note: >-\n      The install advertises Authorization and X-WP-Nonce as acceptable request headers — the standard\n      WordPress cookie+nonce and application-password paths — but neither is obtainable by a third\n      party, since juvlabs.com publishes no signup, no developer portal and no credential issuance.\nverified_anonymous:\n- route: /wp/v2/posts\n  status: 200\n- route: /wp/v2/pages\n  status: 200\n- route: /wp/v2/media\n  status: 200\n- route: /wp/v2/categories\n  status: 200\n- route: /wp/v2/tags\n  status: 200\n- route: /wp/v2/comments\n  status: 200\n- route: /wp/v2/search\n  status: 200\n- route: /wp/v2/types\n  status: 200\n- route: /wp/v2/taxonomies\n\
  \  status: 200\n- route: /wp/v2/statuses\n  status: 200\n- route: /wp/v2/portfolio\n  status: 200\n- route: /wp/v2/portfolio_category\n  status: 200\n- route: /oembed/1.0/embed\n  status: 200\n- route: /wp/v2 (namespace index)\n  status: 200\n- route: / (site index)\n  status: 200\ncredentialed_only:\n- route: /wp/v2/users\n  status: 403\n  code: aios_user_lists_forbidden\n  note: >-\n    User enumeration is explicitly blocked by the All In One Security plugin rather than merely\n    unauthorised — a deliberate hardening choice worth crediting.\n- route: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- route: /wp/v2/plugins\n  status: 401\n  code: rest_cannot_view_plugins\n- route: /wp/v2/themes\n  status: 401\n  code: rest_cannot_view_themes\n- route: /wp/v2/block-types\n  status: 401\n  code: rest_block_type_cannot_view\n- route: /wp/v2/menu-locations\n  status: 401\n  code: rest_cannot_view\n- route: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  note:\
  \ >-\n    The WordPress Abilities API namespace IS registered on this install — the agent-facing capability\n    registry that the WordPress MCP adapter exposes as tools — but an anonymous GET is refused, so the\n    published ability set could not be enumerated. Recorded, not guessed. See mcp/juvenescence-mcp.yml.\n- route: /wp-abilities/v1/categories\n  status: 401\n  code: rest_forbidden\nwrite_operations:\n  modelled: false\n  note: >-\n    POST/PUT/PATCH/DELETE are registered on the content routes but are authenticated administrative\n    endpoints for site editors, not a public API offering. They are deliberately excluded from the\n    OpenAPI in this repository.\nretired_credentialed_api:\n  name: HydraScreen API\n  scheme: http-bearer\n  bearer_format: JWT\n  flow: >-\n    POST /v2/email/verify with an email and organisation; the service mails back a base64-encoded JWT\n    which the client decodes and sends as `Authorization: Bearer <token>`.\n  base_url: https://hydrascreen-api.ro5.ai/v2\n\
  \  source: https://github.com/Ro5-ai/hydrascreen/blob/HEAD/hydrascreen/api.py\n  status: host-does-not-resolve\n  note: >-\n    Documented from the first-party open-source client only, and recorded here for completeness. The\n    host returned NXDOMAIN on 2026-08-23, so this is a historical auth model, not a callable one. No\n    OpenAPI is emitted for it — see lifecycle/juvenescence-lifecycle.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/authentication/juvenescence-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Longevity
- Drug Discovery
- Life Sciences
- Clinical Trials
- Artificial Intelligence
- Aging
- content-api
---
