---
api_key_in: []
api_specs:
- filename: star-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Star Therapeutics Comments API
  slug: star-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-comments-api-openapi.yml
- filename: star-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Star Therapeutics Custom Types API
  slug: star-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-custom-types-api-openapi.yml
- filename: star-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Star Therapeutics Discovery API
  slug: star-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-discovery-api-openapi.yml
- filename: star-therapeutics-media-api-openapi.yml
  format: yaml
  label: Star Therapeutics Media API
  slug: star-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-media-api-openapi.yml
- filename: star-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Star Therapeutics Oembed API
  slug: star-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-oembed-api-openapi.yml
- filename: star-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Star Therapeutics Pages API
  slug: star-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-pages-api-openapi.yml
- filename: star-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Star Therapeutics Posts API
  slug: star-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-posts-api-openapi.yml
- filename: star-therapeutics-search-api-openapi.yml
  format: yaml
  label: Star Therapeutics Search API
  slug: star-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-search-api-openapi.yml
- filename: star-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Star Therapeutics Taxonomy API
  slug: star-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Star Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Star Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Star Therapeutics
provider_slug: star-therapeutics
scheme_count: 0
schemes: []
slug: star-therapeutics-authentication
source_filename: star-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/star-therapeutics-content-openapi.yml + live anonymous probes of https://star-therapeutics.com/wp-json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Star Therapeutics content API declares no security schemes and requires no credentials for\n  any operation catalogued in this repo. The WordPress REST index at /wp-json/ reports an empty\n  `authentication` array, which means no authentication provider (application passwords over\n  Basic, OAuth 1.0a, JWT) is registered for discovery on this deployment. Star Therapeutics\n  publishes no developer authentication documentation because it runs no developer program; the\n  read surface is simply open.\nschemes: []\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n\
  \  - GET /wp/v2/tags\n  - GET /wp/v2/avada_faq\n  - GET /wp/v2/avada_portfolio\n  - GET /wp/v2/faq_category\n  - GET /wp/v2/portfolio_category\n  - GET /wp/v2/blocks\n  - GET /wp/v2/comments\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/statuses\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/users\n    status: 401\n    code: rest_user_cannot_view\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/icons\n    status: 401\n    code: rest_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n\
  \  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  - path: /jet-engine/v1/mcp\n    status: 401\n    code: rest_forbidden\n    note: JSON-RPC tools/list POST also returned 401.\n  - path: /jet-engine/v1/mcp-tools\n    status: 401\n    code: rest_forbidden\n  - path: /gravitykit/v1/abilities\n    status: 401\n    code: rest_forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 491-route index requires an authenticated WordPress\n    user. None were exercised — the pipeline reads only.\nx-evidence:\n  probed: '2026-08-05'\n  index: https://star-therapeutics.com/wp-json/\n  index_authentication_field: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/authentication/star-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Hematology
- Immunology
- Rare Disease
- Antibody Therapeutics
- Clinical Trials
- Life Sciences
- content-api
---
