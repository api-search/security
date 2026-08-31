---
api_key_in: []
api_specs:
- filename: sinclair-broadcast-group-corporate-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Corporate API
  slug: sinclair-broadcast-group-corporate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-corporate-api-openapi.yml
- filename: sinclair-broadcast-group-embed-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Embed API
  slug: sinclair-broadcast-group-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-embed-api-openapi.yml
- filename: sinclair-broadcast-group-media-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Media API
  slug: sinclair-broadcast-group-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-media-api-openapi.yml
- filename: sinclair-broadcast-group-press-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Press API
  slug: sinclair-broadcast-group-press-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-press-api-openapi.yml
- filename: sinclair-broadcast-group-schema-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Schema API
  slug: sinclair-broadcast-group-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-schema-api-openapi.yml
- filename: sinclair-broadcast-group-search-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Search API
  slug: sinclair-broadcast-group-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-search-api-openapi.yml
- filename: sinclair-broadcast-group-stations-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Stations API
  slug: sinclair-broadcast-group-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-stations-api-openapi.yml
- filename: sinclair-broadcast-group-taxonomy-api-openapi.yml
  format: yaml
  label: Sinclair, Inc. Taxonomy API
  slug: sinclair-broadcast-group-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sinclair Broadcast Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sinclair, Inc. declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Sinclair, Inc.
provider_slug: sinclair-broadcast-group
scheme_count: 0
schemes: []
slug: sinclair-broadcast-group-authentication
source_filename: sinclair-broadcast-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Live unauthenticated requests against https://sbgi.net/wp-json/ on 2026-08-12,\n  plus the route index at openapi/_original/sinclair-broadcast-group-wp-json-index.json\nsummary: >-\n  Sinclair declares no security scheme. The WordPress REST API index at\n  https://sbgi.net/wp-json/ reports \"authentication\": [] — meaning no\n  authentication provider is registered for third-party use — and the public\n  content routes answer anonymously with HTTP 200. Privileged routes are still\n  routed and still advertised in the index, but reject anonymous callers with\n  HTTP 401. There is no API key, no OAuth, no token endpoint, no developer\n  signup and no documented way for an outside developer to obtain credentials.\napis:\n  - name: Sinclair Corporate Content API\n    baseURL: https://sbgi.net/wp-json\n    public_read: true\n    credentials_obtainable_by_third_parties: false\n    schemes: []\n    schemes_note: >-\n      The\
  \ derived OpenAPI carries no securitySchemes because the live route\n      descriptors declare none. This is an accurate absence, not a gap in the\n      derivation.\n    observed:\n      - surface: public content read\n        auth_required: false\n        evidence:\n          - url: https://sbgi.net/wp-json/wp/v2/posts?per_page=1\n            status: 200\n          - url: https://sbgi.net/wp-json/sbg/v1/station-map\n            status: 200\n          - url: https://sbgi.net/wp-json/sbg/v1/rsn-map\n            status: 200\n          - url: https://sbgi.net/wp-json/wp/v2/search?search=nextgen\n            status: 200\n      - surface: privileged / administrative\n        auth_required: true\n        mechanism: >-\n          WordPress core session auth (login cookie plus an X-WP-Nonce header) or\n          Application Passwords over HTTP Basic. Neither is offered to third\n          parties by Sinclair; both are editorial-staff mechanisms.\n        error_code_observed: rest_forbidden /\
  \ rest_user_cannot_view / rest_cannot_view_plugins\n        evidence:\n          - url: https://sbgi.net/wp-json/wp/v2/users?per_page=1\n            status: 401\n          - url: https://sbgi.net/wp-json/wp/v2/settings\n            status: 401\n          - url: https://sbgi.net/wp-json/wp/v2/plugins\n            status: 401\n    transport_security:\n      https_only: true\n      hsts: true\n      hsts_max_age: 15768000\n      tls_version: TLSv1.3\n    browser_access:\n      cors_allow_origin: https://sbgi.net\n      third_party_browser_calls: blocked\n      note: >-\n        Access-Control-Allow-Origin is pinned to https://sbgi.net, so a browser on\n        any other origin cannot read this API. Server-side callers are unaffected.\n        This is the practical access constraint on the surface, not authentication.\n      evidence:\n        - url: https://sbgi.net/wp-json/wp/v2/posts?per_page=2\n          header: 'access-control-allow-origin: https://sbgi.net'\n          status: 200\n \
  \   accepted_headers:\n      - Authorization\n      - X-WP-Nonce\n      - Content-Disposition\n      - Content-MD5\n      - Content-Type\n    oauth2: false\n    openid_connect: false\n    api_keys: false\n    mutual_tls: false\ndocs: null\ndocs_note: >-\n  Sinclair publishes no authentication documentation. The mechanisms above are the\n  WordPress core defaults observed on this host, not a Sinclair-published contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/authentication/sinclair-broadcast-group-authentication.yml
summary_line: 0 schemes
tags:
- Broadcasting
- Television
- Local News
- Sports Media
- Regional Sports Networks
- Digital Marketing
- Advertising Technology
- NextGen TV
- ATSC 3.0
- Media
---
