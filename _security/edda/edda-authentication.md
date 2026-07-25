---
api_key_in: []
api_specs:
- filename: edda-categories-api-openapi.yml
  format: yaml
  label: EDDA Technology categories API
  slug: edda-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-categories-api-openapi.yml
- filename: edda-comments-api-openapi.yml
  format: yaml
  label: EDDA Technology comments API
  slug: edda-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-comments-api-openapi.yml
- filename: edda-embed-api-openapi.yml
  format: yaml
  label: EDDA Technology embed API
  slug: edda-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-embed-api-openapi.yml
- filename: edda-media-api-openapi.yml
  format: yaml
  label: EDDA Technology media API
  slug: edda-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-media-api-openapi.yml
- filename: edda-pages-api-openapi.yml
  format: yaml
  label: EDDA Technology pages API
  slug: edda-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-pages-api-openapi.yml
- filename: edda-posts-api-openapi.yml
  format: yaml
  label: EDDA Technology posts API
  slug: edda-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-posts-api-openapi.yml
- filename: edda-search-api-openapi.yml
  format: yaml
  label: EDDA Technology search API
  slug: edda-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-search-api-openapi.yml
- filename: edda-statuses-api-openapi.yml
  format: yaml
  label: EDDA Technology statuses API
  slug: edda-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-statuses-api-openapi.yml
- filename: edda-tags-api-openapi.yml
  format: yaml
  label: EDDA Technology tags API
  slug: edda-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-tags-api-openapi.yml
- filename: edda-taxonomies-api-openapi.yml
  format: yaml
  label: EDDA Technology taxonomies API
  slug: edda-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-taxonomies-api-openapi.yml
- filename: edda-types-api-openapi.yml
  format: yaml
  label: EDDA Technology types API
  slug: edda-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-types-api-openapi.yml
- filename: edda-users-api-openapi.yml
  format: yaml
  label: EDDA Technology users API
  slug: edda-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-users-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: searched
name: Edda Authentication
name_suffix: Authentication
oauth_flows: []
overview: EDDA Technology secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EDDA Technology
provider_slug: edda
scheme_count: 2
schemes:
- description: All read operations catalogued in openapi/edda-wordpress-openapi.yml return 200 with no Authorization header. Verified live 2026-07-20.
  name: anonymous
  sources:
  - openapi/edda-wordpress-openapi.yml
  type: none
- accepted_headers:
  - Authorization
  - X-WP-Nonce
  applies_to: write operations and non-public routes (e.g. /wp/v2/settings, /mpdl/downloads/files)
  authorization_endpoint: https://www.eddatech.com/wp-admin/authorize-application.php
  description: 'WordPress application passwords (HTTP Basic: username + application password). Advertised by the API root at https://www.eddatech.com/wp-json/ under authentication.application-passwords. Credentials are issued per WordPress user account by the site administrator, not through a public developer program. Required only for write operations and non-public routes.'
  name: applicationPassword
  scheme: basic
  sources:
  - https://www.eddatech.com/wp-json/
  - openapi/edda-wordpress-openapi.yml
  type: http
slug: edda-authentication
source_filename: edda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.eddatech.com/wp-json/\ndocs: https://www.eddatech.com/wp-json/\nsummary:\n  types:\n  - none\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\n  notes: >-\n    EDDA Technology publishes no developer-facing authentication program. The only public HTTP API\n    surface is the WordPress REST API on www.eddatech.com, whose entire public read surface\n    (posts, pages, media, taxonomies, search, oEmbed) is served anonymously with no credential.\n    The API root advertises exactly one authentication mechanism — WordPress application passwords\n    (HTTP Basic) — which gates write operations and administrative routes and is not offered to\n    third-party developers. There is no OAuth 2.0, no OpenID Connect, no API-key program and no\n    developer key issuance, so scopes/ is intentionally absent.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    All read operations catalogued\
  \ in openapi/edda-wordpress-openapi.yml return 200 with no\n    Authorization header. Verified live 2026-07-20.\n  sources:\n  - openapi/edda-wordpress-openapi.yml\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords (HTTP Basic: username + application password). Advertised by the\n    API root at https://www.eddatech.com/wp-json/ under authentication.application-passwords.\n    Credentials are issued per WordPress user account by the site administrator, not through a public\n    developer program. Required only for write operations and non-public routes.\n  authorization_endpoint: https://www.eddatech.com/wp-admin/authorize-application.php\n  accepted_headers:\n  - Authorization\n  - X-WP-Nonce\n  applies_to: write operations and non-public routes (e.g. /wp/v2/settings, /mpdl/downloads/files)\n  sources:\n  - https://www.eddatech.com/wp-json/\n  - openapi/edda-wordpress-openapi.yml\nobserved:\n- request: GET https://www.eddatech.com/wp-json/wp/v2/posts?per_page=1\n\
  \  auth: none\n  status: 200\n- request: GET https://www.eddatech.com/wp-json/wp/v2/settings\n  auth: none\n  status: 401\n  body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n- request: GET https://www.eddatech.com/wp-json/mpdl/downloads/files\n  auth: none\n  status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/authentication/edda-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Health Tech
- Medical Imaging
- Radiology
- Surgery
- Oncology
- Artificial Intelligence
- Medical Devices
- Healthcare
- Clinical Software
---
