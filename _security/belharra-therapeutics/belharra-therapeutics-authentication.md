---
api_key_in: []
api_specs:
- filename: belharra-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Custom Types API
  slug: belharra-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-custom-types-api-openapi.yml
- filename: belharra-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Discovery API
  slug: belharra-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-discovery-api-openapi.yml
- filename: belharra-therapeutics-media-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Media API
  slug: belharra-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-media-api-openapi.yml
- filename: belharra-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Oembed API
  slug: belharra-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-oembed-api-openapi.yml
- filename: belharra-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Pages API
  slug: belharra-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-pages-api-openapi.yml
- filename: belharra-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Posts API
  slug: belharra-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-posts-api-openapi.yml
- filename: belharra-therapeutics-search-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Search API
  slug: belharra-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-search-api-openapi.yml
- filename: belharra-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Taxonomy API
  slug: belharra-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Belharra Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Belharra Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Belharra Therapeutics
provider_slug: belharra-therapeutics
scheme_count: 0
schemes: []
slug: belharra-therapeutics-authentication
source_filename: belharra-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/belharra-therapeutics-content-openapi.yml + live anonymous probes of https://belharratx.com/wp-json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Belharra Therapeutics content API declares no security schemes and requires no credentials\n  for any operation catalogued in this repo. The WordPress REST index at /wp-json/ does advertise\n  one authentication provider for discovery — WordPress application passwords, with an\n  authorization endpoint at https://belharratx.com/wp-admin/authorize-application.php — but that is\n  the WordPress core admin credential flow for authenticated site users, not a developer\n  authentication scheme Belharra publishes for API consumers. It is recorded below for accuracy and\n  is deliberately NOT modelled as a securityScheme in the OpenAPI, because no operation in this\n  repo uses it and no consumer can obtain such a credential. Belharra\
  \ publishes no developer\n  authentication documentation because it runs no developer program; the read surface is simply\n  open.\nschemes: []\nadvertised_by_index:\n- name: application-passwords\n  kind: wordpress-core-admin\n  authorization_endpoint: https://belharratx.com/wp-admin/authorize-application.php\n  transport: HTTP Basic over TLS\n  available_to_public: false\n  detail: >-\n    Reported in the `authentication` object of the /wp-json/ index. Requires an existing WordPress\n    user account on this installation, which is issued only to Belharra staff. No self-service\n    registration exists — https://belharratx.com/wp-login.php is the only entry point.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/press-release\n  - GET /wp/v2/press-release/{id}\n  - GET /wp/v2/company-news\n  - GET /wp/v2/company-news/{id}\n  - GET /wp/v2/multimedia-file\n  - GET /wp/v2/multimedia-file/{id}\n\
  \  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/search\n  - GET /wp/v2/users\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/statuses\n  - GET /wp/v2/blocks\n  - GET /wp/v2/navigation\n  - GET /oembed/1.0/embed\n  readable_but_empty:\n  - path: /wp/v2/tags\n    x_wp_total: 0\n    note: The post_tag taxonomy is registered but carries no terms.\n  - path: /wp/v2/blocks\n    x_wp_total: 0\n  - path: /wp/v2/navigation\n    x_wp_total: 0\n  gated:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/menu-locations\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n\
  \  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/icons\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/sidebars\n    status: 401\n    code: rest_cannot_manage_widgets\n  - path: /wp/v2/widget-types\n    status: 401\n    code: rest_cannot_manage_widgets\n  - path: /wp/v2/templates\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/template-parts\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/global-styles/themes/{stylesheet}\n    status: 401\n    code: rest_cannot_read_global_styles\n  - path: /wp/v2/block-patterns/patterns\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/block-patterns/categories\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/pattern-directory/patterns\n    status: 401\n    code: rest_pattern_directory_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress\
  \ Abilities API — an agent-facing capability registry. Gated, so no MCP or agent\n      surface is claimed for this provider.\n  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  - path: /wp-site-health/v1/directory-sizes\n    status: 401\n    code: rest_forbidden\n  - path: /wp-block-editor/v1/navigation-fallback\n    status: 401\n    code: rest_cannot_create\n  - path: /podcastplayer/v1/posttypes\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/comments\n    status: 403\n    code: rest_comment_disabled\n    note: Commenting is switched off site-wide, so the collection is refused rather than empty.\n  - path: /contact-form-7/v1/contact-forms\n    status: 403\n    code: wpcf7_forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 198-route index requires an authenticated WordPress\n    user. None were exercised — the pipeline reads only.\nx-evidence:\n  probed: '2026-08-06'\n  index: https://belharratx.com/wp-json/\n\
  \  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://belharratx.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/authentication/belharra-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- biotechnology
- pharmaceuticals
- chemoproteomics
- drug-discovery
- small-molecule-therapeutics
- proteomics
- life-sciences
- oncology
- immunology
- content-api
---
