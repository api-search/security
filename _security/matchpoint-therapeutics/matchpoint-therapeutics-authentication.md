---
api_key_in: []
api_specs:
- filename: matchpoint-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Comments API
  slug: matchpoint-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-comments-api-openapi.yml
- filename: matchpoint-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Discovery API
  slug: matchpoint-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-discovery-api-openapi.yml
- filename: matchpoint-therapeutics-media-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Media API
  slug: matchpoint-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-media-api-openapi.yml
- filename: matchpoint-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Oembed API
  slug: matchpoint-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-oembed-api-openapi.yml
- filename: matchpoint-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Pages API
  slug: matchpoint-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-pages-api-openapi.yml
- filename: matchpoint-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Posts API
  slug: matchpoint-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-posts-api-openapi.yml
- filename: matchpoint-therapeutics-search-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Search API
  slug: matchpoint-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-search-api-openapi.yml
- filename: matchpoint-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Taxonomy API
  slug: matchpoint-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-taxonomy-api-openapi.yml
- filename: matchpoint-therapeutics-team-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Team API
  slug: matchpoint-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-team-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Matchpoint Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matchpoint Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Matchpoint Therapeutics
provider_slug: matchpoint-therapeutics
scheme_count: 0
schemes: []
slug: matchpoint-therapeutics-authentication
source_filename: matchpoint-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: >-\n  openapi/*.yml in this repo + live anonymous probes of https://matchpointtx.com/wp-json on\n  2026-08-25\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Matchpoint Therapeutics content API declares no security schemes and requires no credentials\n  for any operation catalogued in this repo. The WordPress REST index at /wp-json/ reports an empty\n  `authentication` array, which means no authentication provider (application passwords over Basic,\n  OAuth 1.0a, JWT) is registered for discovery on this deployment. Matchpoint publishes no developer\n  authentication documentation because it runs no developer program; the read surface is simply\n  open, and everything that is not open is closed to an authenticated WordPress user rather than to\n  an API consumer. `0-working/derive-authentication.py` produced no profile for this provider\n  precisely because there is no securityScheme\
  \ to derive one from — that absence is the finding.\nschemes: []\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/team\n  - GET /wp/v2/team/{id}\n  - GET /wp/v2/team_types\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/comments\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/types/{type}\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/taxonomies/{taxonomy}\n  - GET /wp/v2/statuses\n  - GET /wp/v2/statuses/{status}\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/users\n    status: 401\n    code: rest_user_cannot_view\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/menu-items\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/themes\n \
  \   status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/icons\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/templates\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/template-parts\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/sidebars\n    status: 401\n    code: rest_cannot_manage_widgets\n  - path: /wp/v2/widget-types\n    status: 401\n    code: rest_cannot_manage_widgets\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities API — the core surface an MCP bridge would expose. Registered on this\n      deployment but closed to anonymous callers, so no agent-callable tool list is reachable.\n\
  \  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  - path: /struck/v1/logs\n    status: 401\n    code: rest_forbidden\n  - path: /struck/v1/ssl\n    status: 401\n    code: rest_forbidden\n  - path: /oembed/1.0/proxy\n    status: 401\n    code: rest_forbidden\n  - path: /acf/v3/options/{option_name}\n    status: 403\n    code: forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 222-route index requires an authenticated WordPress\n    user. None were exercised — the pipeline reads only. /customgf/v2/forms/{id}/submissions is the\n    single anonymous-write candidate on the deployment (a Gravity Forms submission endpoint); it was\n    NOT exercised, and the sibling GET /customgf/v2/forms/1 returned HTTP 500, so no form id is\n    known to be valid.\nx-evidence:\n  probed: '2026-08-25'\n  index: https://matchpointtx.com/wp-json/\n  index_authentication_field: []\n  namespaces: 13\n  routes: 222\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/authentication/matchpoint-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Immunology
- Covalent Chemistry
- Chemoproteomics
- Machine Learning
- Life Sciences
- content-api
---
