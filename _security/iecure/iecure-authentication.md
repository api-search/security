---
api_key_in: []
api_specs:
- filename: iecure-discovery-api-openapi.yml
  format: yaml
  label: iECURE Discovery API
  slug: iecure-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-discovery-api-openapi.yml
- filename: iecure-posts-api-openapi.yml
  format: yaml
  label: iECURE Posts API
  slug: iecure-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-posts-api-openapi.yml
- filename: iecure-pages-api-openapi.yml
  format: yaml
  label: iECURE Pages API
  slug: iecure-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-pages-api-openapi.yml
- filename: iecure-media-api-openapi.yml
  format: yaml
  label: iECURE Media API
  slug: iecure-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-media-api-openapi.yml
- filename: iecure-taxonomy-api-openapi.yml
  format: yaml
  label: iECURE Taxonomy API
  slug: iecure-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-taxonomy-api-openapi.yml
- filename: iecure-team-api-openapi.yml
  format: yaml
  label: iECURE Team API
  slug: iecure-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-team-api-openapi.yml
- filename: iecure-search-api-openapi.yml
  format: yaml
  label: iECURE Search API
  slug: iecure-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-search-api-openapi.yml
- filename: iecure-users-api-openapi.yml
  format: yaml
  label: iECURE Authors API
  slug: iecure-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-users-api-openapi.yml
- filename: iecure-comments-api-openapi.yml
  format: yaml
  label: iECURE Comments API
  slug: iecure-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-comments-api-openapi.yml
- filename: iecure-oembed-api-openapi.yml
  format: yaml
  label: iECURE oEmbed API
  slug: iecure-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-oembed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Iecure Authentication
name_suffix: Authentication
oauth_flows: []
overview: iECURE secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iECURE
provider_slug: iecure
scheme_count: 1
schemes:
- applies_to: Authenticated WordPress users only; no anonymous route requires or accepts it.
  authorization_endpoint: https://iecure.com/wp-admin/authorize-application.php
  declared_in: https://iecure.com/wp-json/ (authentication.application-passwords)
  detail: WordPress Application Passwords. The user authorizes an application at the wp-admin URL above and receives a generated password sent as HTTP Basic credentials. No scopes, no expiry contract, no refresh. iECURE does not document this and it is not offered to third parties.
  name: applicationPasswords
  scheme: basic
  type: http
slug: iecure-authentication
source_filename: iecure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: openapi/ + live anonymous probes of https://iecure.com/wp-json on 2026-08-22\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  iECURE runs no developer program and publishes no authentication documentation. Every operation\n  catalogued in this repo is anonymous read: no credentials are required and none are accepted for\n  the content collections. The /wp-json/ index does, however, advertise one authentication provider\n  — WordPress Application Passwords, presented over HTTP Basic — whose authorization endpoint is the\n  wp-admin screen. That is an editorial credential for staff, not a developer credential: there is no\n  self-service sign-up, no key issuance, and no scope model behind it. It is recorded here because it\n  is what the provider's own discovery document declares, not because it is a consumable auth surface.\nschemes:\n- name: applicationPasswords\n  type: http\n\
  \  scheme: basic\n  declared_in: https://iecure.com/wp-json/ (authentication.application-passwords)\n  authorization_endpoint: https://iecure.com/wp-admin/authorize-application.php\n  applies_to: Authenticated WordPress users only; no anonymous route requires or accepts it.\n  detail: >-\n    WordPress Application Passwords. The user authorizes an application at the wp-admin URL above and\n    receives a generated password sent as HTTP Basic credentials. No scopes, no expiry contract, no\n    refresh. iECURE does not document this and it is not offered to third parties.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/portfolio\n  - GET /wp/v2/portfolio/{id}\n  - GET /wp/v2/portfolio_entries\n  - GET /wp/v2/portfolio_entries/{id}\n  - GET\
  \ /wp/v2/comments\n  - GET /wp/v2/users\n  - GET /wp/v2/users/{id}\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/types/{type}\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/taxonomies/{taxonomy}\n  - GET /wp/v2/statuses\n  - GET /wp/v2/statuses/{status}\n  - GET /wp/v2/blocks\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/menu-locations\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/sidebars\n    status: 401\n    code: rest_cannot_manage_widgets\n  - path: /wp/v2/font-collections\n    status: 401\n    code: rest_cannot_read\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities\
  \ API — the agent-facing capability registry that MCP adapters read.\n      Registered on this deployment but closed to anonymous callers.\n  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  - path: /aioseo/v1/ping\n    status: 401\n    code: rest_forbidden\n  - path: /aioseo/v1/tags\n    status: 401\n    code: rest_forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 351-route index requires an authenticated WordPress\n    user. None were exercised — this pipeline reads only.\nx-evidence:\n  probed: '2026-08-22'\n  index: https://iecure.com/wp-json/\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://iecure.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/authentication/iecure-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- biotechnology
- genetic-medicine
- gene-editing
- gene-therapy
- rare-disease
- clinical-trials
- life-sciences
- pharmaceuticals
- content-api
---
