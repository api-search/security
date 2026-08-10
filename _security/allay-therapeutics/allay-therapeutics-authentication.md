---
api_key_in: []
api_specs:
- filename: allay-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Comments API
  slug: allay-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-comments-api-openapi.yml
- filename: allay-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Discovery API
  slug: allay-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-discovery-api-openapi.yml
- filename: allay-therapeutics-media-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Media API
  slug: allay-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-media-api-openapi.yml
- filename: allay-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Oembed API
  slug: allay-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-oembed-api-openapi.yml
- filename: allay-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Pages API
  slug: allay-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-pages-api-openapi.yml
- filename: allay-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Posts API
  slug: allay-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-posts-api-openapi.yml
- filename: allay-therapeutics-search-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Search API
  slug: allay-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-search-api-openapi.yml
- filename: allay-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Allay Therapeutics Taxonomy API
  slug: allay-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/openapi/allay-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Allay Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allay Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Allay Therapeutics
provider_slug: allay-therapeutics
scheme_count: 0
schemes: []
slug: allay-therapeutics-authentication
source_filename: allay-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/allay-therapeutics-content-openapi.yml + live anonymous probes of https://www.allaytx.com/wp-json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Allay Therapeutics content API declares no security schemes and requires no credentials for\n  any operation catalogued in this repo. The WordPress REST index at /wp-json/ advertises exactly\n  one authentication method — WordPress application passwords, with an authorization endpoint at\n  https://www.allaytx.com/wp-admin/authorize-application.php — which is an administrative CMS\n  sign-in flow for site editors, not a consumer API credential: there is no self-service signup, no\n  key issuance, no scopes and no documentation. Allay Therapeutics publishes no developer\n  authentication documentation because it runs no developer program; the read surface is simply\n  open.\nschemes: []\nadvertised_by_index:\n- method: application-passwords\n\
  \  mechanism: HTTP Basic with an admin-issued application password\n  authorization_endpoint: https://www.allaytx.com/wp-admin/authorize-application.php\n  consumer_available: false\n  detail: >-\n    WordPress core's application-password flow. Requires an existing WordPress user account on this\n    site; there is no public registration path. Not modelled as an OpenAPI securityScheme because\n    no catalogued operation accepts or requires it.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/tags/{id}\n  - GET /wp/v2/comments\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/statuses\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n\
  \    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp/v2/icons\n    status: 401\n    code: rest_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      WordPress core's agent-capability registry. Gated, so no MCP or agent-tool surface is claimed\n      for this provider.\n  open_but_excluded:\n  - path: /wp/v2/users\n    status: 200\n    detail: >-\n      Author enumeration is left open on this deployment — the collection returns 7 author records\n      anonymously. Recorded as an observed exposure, deliberately not modelled as an operation and\n      deliberately not packaged as an agent skill or MCP tool.\
  \ No individual is named in this\n      repository.\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 196-route index requires an authenticated WordPress\n    user. None were exercised — the pipeline reads only.\nx-evidence:\n  probed: '2026-08-06'\n  index: https://www.allaytx.com/wp-json/\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://www.allaytx.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/authentication/allay-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Pain Management
- Drug Delivery
- Non-Opioid
- Clinical Stage
- Health
- Life Sciences
- content-api
---
