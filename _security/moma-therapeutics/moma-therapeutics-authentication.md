---
api_key_in: []
api_specs:
- filename: moma-therapeutics-posts-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Content Posts API
  slug: moma-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-posts-api-openapi.yml
- filename: moma-therapeutics-pages-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Content Pages API
  slug: moma-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-pages-api-openapi.yml
- filename: moma-therapeutics-team-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Team API
  slug: moma-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-team-api-openapi.yml
- filename: moma-therapeutics-media-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Media API
  slug: moma-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-media-api-openapi.yml
- filename: moma-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Taxonomy API
  slug: moma-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-taxonomy-api-openapi.yml
- filename: moma-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Discovery API
  slug: moma-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-discovery-api-openapi.yml
- filename: moma-therapeutics-search-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Search API
  slug: moma-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-search-api-openapi.yml
- filename: moma-therapeutics-comments-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Comments API
  slug: moma-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-comments-api-openapi.yml
- filename: moma-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics oEmbed API
  slug: moma-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-oembed-api-openapi.yml
- filename: moma-therapeutics-options-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Site Options API
  slug: moma-therapeutics-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-options-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Moma Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: MOMA Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MOMA Therapeutics
provider_slug: moma-therapeutics
scheme_count: 0
schemes: []
slug: moma-therapeutics-authentication
source_filename: moma-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://momatx.com/wp-json/ and its route index on 2026-08-26,\n  read against the upstream WordPress REST authentication contract at\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary: >-\n  MOMA Therapeutics documents no authentication because it documents no API. The WordPress REST\n  content API behind momatx.com is read-anonymous for its published-content routes and refuses\n  everything else with HTTP 401. There is no API key, no OAuth surface, no token issuance, no\n  registration and no self-service path to credentials of any kind.\nadvertised_schemes: []\nadvertised_schemes_note: >-\n  The route index's own `authentication` member is an empty array — the deployment advertises no\n  authentication scheme to clients. WordPress core supports cookie authentication (browser\
  \ session\n  plus an X-WP-Nonce header) and Application Passwords over HTTP Basic; the Application Passwords\n  routes are registered here (/wp/v2/users/{user_id}/application-passwords) but require an\n  existing authenticated user to reach, so they are not an onboarding path for a third party.\nsecurity_schemes: []\nsecurity_schemes_note: >-\n  The derived OpenAPI documents in openapi/ declare no securitySchemes, and that is a faithful\n  description rather than an omission: every operation captured in them was verified to return\n  data with no credential attached.\naccess:\n  anonymous_read: true\n  self_service_signup: false\n  api_keys: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  registration_url: null\n  registration_note: >-\n    No developer registration exists. WordPress account creation is not open on this deployment.\nanonymous_surface:\n- path: /wp/v2/posts\n  status: 200\n- path: /wp/v2/pages\n  status: 200\n- path: /wp/v2/media\n  status: 200\n\
  - path: /wp/v2/team\n  status: 200\n- path: /wp/v2/team_types\n  status: 200\n- path: /wp/v2/categories\n  status: 200\n- path: /wp/v2/tags\n  status: 200\n- path: /wp/v2/comments\n  status: 200\n- path: /wp/v2/search\n  status: 200\n- path: /wp/v2/types\n  status: 200\n- path: /wp/v2/taxonomies\n  status: 200\n- path: /wp/v2/statuses\n  status: 200\n- path: /oembed/1.0/embed\n  status: 200\n- path: /acf/v3/options/options\n  status: 200\ngated_surface:\n- path: /wp/v2/users\n  status: 401\n  code: rest_user_cannot_view\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/menu-items\n  status: 401\n  code: rest_cannot_view\n- path: /wp/v2/plugins\n  status: 401\n  code: rest_cannot_view_plugins\n- path: /wp/v2/themes\n  status: 401\n  code: rest_cannot_view_themes\n- path: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API namespace is registered on this deployment — the surface that\n    exposes site\
  \ capabilities as invocable abilities to agents — but both /abilities and\n    /categories refuse anonymous callers. Its schemas would require authenticated introspection.\n- path: /wp-abilities/v1/categories\n  status: 401\n  code: rest_forbidden\nwrite_operations:\n  available_anonymously: false\n  note: >-\n    Every route in the index that declares POST, PUT, PATCH or DELETE requires an authenticated\n    user with the matching capability. No write operation is reachable without credentials, and\n    none is captured in the OpenAPI documents in this repository.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/authentication/moma-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Oncology
- Precision Medicine
- Life Sciences
- Structural Biology
- Machine Learning
- content-api
---
