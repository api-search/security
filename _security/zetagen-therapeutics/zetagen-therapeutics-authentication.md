---
api_key_in: []
api_specs:
- filename: zetagen-therapeutics-content-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Content API
  slug: zetagen-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-content-api-openapi.yml
- filename: zetagen-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Discovery API
  slug: zetagen-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-discovery-api-openapi.yml
- filename: zetagen-therapeutics-downloads-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Downloads API
  slug: zetagen-therapeutics-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-downloads-api-openapi.yml
- filename: zetagen-therapeutics-embed-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Embed API
  slug: zetagen-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-embed-api-openapi.yml
- filename: zetagen-therapeutics-media-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Media API
  slug: zetagen-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-media-api-openapi.yml
- filename: zetagen-therapeutics-people-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics People API
  slug: zetagen-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-people-api-openapi.yml
- filename: zetagen-therapeutics-search-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Search API
  slug: zetagen-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-search-api-openapi.yml
- filename: zetagen-therapeutics-seo-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Seo API
  slug: zetagen-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-seo-api-openapi.yml
- filename: zetagen-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Taxonomy API
  slug: zetagen-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Zetagen Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zetagen Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Zetagen Therapeutics
provider_slug: zetagen-therapeutics
scheme_count: 0
schemes: []
slug: zetagen-therapeutics-authentication
source_filename: zetagen-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: >-\n  openapi/zetagen-therapeutics-content-openapi.yml + live anonymous probes of\n  https://zetagen.com/wp-json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The Zetagen Therapeutics content API declares no security schemes and requires no credentials for\n  any operation catalogued in this repo. The WordPress REST index at /wp-json/ reports exactly one\n  registered authentication provider — WordPress application passwords, authorised at\n  /wp-admin/authorize-application.php and presented over HTTP Basic — which is the WordPress core\n  default for authenticated write access by the site's own operators. It is not a developer\n  credential a third party can obtain: there is no self-service signup for it, no scope model and no\n  key-issuance flow. Zetagen publishes no developer authentication documentation because it runs no\n  developer program; the read surface is simply open.\n\
  schemes: []\nregistered_providers:\n- name: application-passwords\n  mechanism: HTTP Basic (WordPress application password)\n  authorization_endpoint: https://zetagen.com/wp-admin/authorize-application.php\n  source: the `authentication` object in https://zetagen.com/wp-json/\n  third_party_obtainable: false\n  note: >-\n    WordPress core default. Requires an existing WordPress user account on zetagen.com. Not modelled\n    as a securityScheme in the OpenAPI because no catalogued operation accepts or requires it — the\n    pipeline reads only and never exercised a write route.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/tags/{id}\n  - GET /wp/v2/comments\n  - GET /wp/v2/blocks\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n\
  \  - GET /wp/v2/statuses\n  - GET /oembed/1.0/embed\n  - GET /yoast/v1/get_head\n  - GET /wpdm/search\n  gated:\n  - {path: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/menus, status: 401, code: rest_cannot_view}\n  - {path: /wp/v2/themes, status: 401, code: rest_cannot_view_themes}\n  - {path: /wp/v2/plugins, status: 401, code: rest_cannot_view_plugins}\n  - {path: /wp/v2/block-types, status: 401, code: rest_block_type_cannot_view}\n  - {path: /wp/v2/block-patterns/categories, status: 401, code: rest_cannot_view}\n  - {path: /wp/v2/font-collections, status: 401, code: rest_cannot_read}\n  - {path: /wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\n  - {path: /wp-abilities/v1/categories, status: 401, code: rest_forbidden}\n  - {path: /wp-site-health/v1/tests/background-updates, status: 401, code: rest_forbidden}\n  - {path: /redirection/v1/redirect, status: 401, code: rest_forbidden}\n  - {path: /code-snippets/v1/snippets, status: 401, code: rest_forbidden}\n\
  \  - {path: /akismet/v1/key, status: 401, code: rest_forbidden}\n  personal_data:\n  - path: /wp/v2/users\n    status: 200\n    total: 4\n    note: >-\n      The standard WordPress author collection answers anonymously on this deployment, exposing\n      author display names, slugs and avatar URLs (not email addresses). Documented in the OpenAPI\n      as x-personal-data and deliberately excluded from every packaged Agent Skill. No response data\n      was captured and no individual is named anywhere in this repo. See review.yml.\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 349-route index requires an authenticated WordPress\n    user. None were exercised — the pipeline reads only.\nx-evidence:\n  probed: '2026-08-05'\n  index: https://zetagen.com/wp-json/\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://zetagen.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/authentication/zetagen-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- biopharmaceuticals
- Oncology
- Bone Health
- Orthopedics
- Clinical Trials
- Life Sciences
- Drug Development
- Medical Devices
- content-api
---
