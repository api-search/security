---
api_key_in: []
api_specs:
- filename: edda-wordpress-openapi.yml
  format: yaml
  label: EDDA Technology WordPress REST API
  slug: wordpress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-wordpress-openapi.yml
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
