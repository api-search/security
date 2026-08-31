---
api_key_in: []
api_specs:
- filename: flare-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Comments API
  slug: flare-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-comments-api-openapi.yml
- filename: flare-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Discovery API
  slug: flare-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-discovery-api-openapi.yml
- filename: flare-therapeutics-media-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Media API
  slug: flare-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-media-api-openapi.yml
- filename: flare-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Oembed API
  slug: flare-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-oembed-api-openapi.yml
- filename: flare-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Pages API
  slug: flare-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-pages-api-openapi.yml
- filename: flare-therapeutics-patterns-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Patterns API
  slug: flare-therapeutics-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-patterns-api-openapi.yml
- filename: flare-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Posts API
  slug: flare-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-posts-api-openapi.yml
- filename: flare-therapeutics-search-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Search API
  slug: flare-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-search-api-openapi.yml
- filename: flare-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Taxonomy API
  slug: flare-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Flare Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flare Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Flare Therapeutics
provider_slug: flare-therapeutics
scheme_count: 0
schemes: []
slug: flare-therapeutics-authentication
source_filename: flare-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: >-\n  openapi/flare-therapeutics-content-openapi.yml + live anonymous probes of\n  https://www.flaretx.com/wp-json on 2026-08-12\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Flare Therapeutics content API declares no security schemes and requires no credentials for\n  any operation catalogued in this repo. The WordPress REST index at /wp-json/ advertises exactly\n  one authentication provider — WordPress application passwords over HTTP Basic, with the\n  authorization screen at /wp-admin/authorize-application.php — which is the WordPress core\n  admin-user credential flow, not a developer-facing API key programme. There is no key issuance, no\n  registration, no scope model and no developer documentation, because Flare Therapeutics runs no\n  developer program. The read surface is simply open; everything else is closed to a WordPress user\n  account.\nschemes: []\nadvertised_provider:\n\
  \  name: application-passwords\n  mechanism: HTTP Basic with a WordPress user + application password\n  authorization_endpoint: https://www.flaretx.com/wp-admin/authorize-application.php\n  source: the `authentication` object in the /wp-json/ route index\n  detail: >-\n    WordPress core default. Grants an existing WordPress user's own capabilities; it is not a\n    third-party developer credential and confers no access a member of the public can obtain. Not\n    modelled as a securityScheme in the OpenAPI because no operation in that document requires it.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/comments\n  - GET /wp/v2/blocks\n  - GET /wp/v2/wp_pattern_category\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/types/{type}\n\
  \  - GET /wp/v2/taxonomies\n  - GET /wp/v2/taxonomies/{taxonomy}\n  - GET /wp/v2/statuses\n  - GET /wp/v2/statuses/{status}\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/users\n    status: 401\n    code: rest_cannot_access\n    message: Only authenticated users can access the User endpoint REST API.\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/icons\n    status: 401\n    code: rest_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n\
  \  - path: /oembed/1.0/proxy\n    status: 401\n    code: rest_forbidden\n    note: The oEmbed proxy is closed; only the provider endpoint /oembed/1.0/embed is open.\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 259-route index requires an authenticated WordPress\n    user — including the plugin namespaces aiarc/v1 (upload, crop), post-duplicator/v1,\n    mtphrSettings/v1 and gosmtp-smtp. None were exercised; the pipeline reads only.\nx-evidence:\n  probed: '2026-08-12'\n  index: https://www.flaretx.com/wp-json/\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://www.flaretx.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/authentication/flare-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Precision Medicine
- transcription-factors
- Drug Discovery
- Clinical Trials
- Life Sciences
- content-api
---
