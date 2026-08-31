---
api_key_in: []
api_specs:
- filename: kallyope-discovery-api-openapi.yml
  format: yaml
  label: Kallyope Discovery API
  slug: kallyope-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-discovery-api-openapi.yml
- filename: kallyope-documents-api-openapi.yml
  format: yaml
  label: Kallyope Documents API
  slug: kallyope-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-documents-api-openapi.yml
- filename: kallyope-media-api-openapi.yml
  format: yaml
  label: Kallyope Media API
  slug: kallyope-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-media-api-openapi.yml
- filename: kallyope-news-api-openapi.yml
  format: yaml
  label: Kallyope News API
  slug: kallyope-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-news-api-openapi.yml
- filename: kallyope-pages-api-openapi.yml
  format: yaml
  label: Kallyope Pages API
  slug: kallyope-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-pages-api-openapi.yml
- filename: kallyope-taxonomies-api-openapi.yml
  format: yaml
  label: Kallyope Taxonomies API
  slug: kallyope-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-taxonomies-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Kallyope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kallyope secures its APIs with none and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kallyope
provider_slug: kallyope
scheme_count: 3
schemes:
- applies_to: all read operations
  description: Every GET collection and item route described in openapi/kallyope-content-api-openapi.yml returned HTTP 200 with real JSON and no credential of any kind. There is no API key, no signup, no token issuance and no per-consumer identity on this surface.
  evidence:
    example: GET https://kallyope.com/wp-json/wp/v2/document?per_page=1 -> 200
    observed: '2026-08-01'
  name: anonymous
  sources:
  - openapi/kallyope-content-api-openapi.yml
  type: none
- audience: internal WordPress users only
  authorization_endpoint: https://kallyope.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, advertised verbatim by the route index `authentication` block. Credentials are minted per WordPress user in the site admin and presented as HTTP Basic. This is the write/administrative path — it is not offered to third parties and no self-service registration exists.
  name: application-passwords
  scheme: basic
  sources:
  - https://kallyope.com/wp-json/
  type: http
- description: 'The stock WordPress logged-in cookie plus an `X-WP-Nonce` header, used by the block editor and admin JavaScript. Advertised indirectly by the `Access-Control-Allow-Headers: Authorization, X-WP-Nonce, ...` response header observed on every route. Browser-session only; not a third-party integration path.'
  in: header
  name: cookie-nonce
  parameter_name: X-WP-Nonce
  sources:
  - https://kallyope.com/wp-json/wp/v2/document
  type: apiKey
slug: kallyope-authentication
source_filename: kallyope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://kallyope.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nnote: >-\n  Kallyope publishes no authentication documentation of its own — there is no developer\n  portal and no API reference. This profile is recorded from the live route index at\n  https://kallyope.com/wp-json/ (whose `authentication` block advertises the mechanism)\n  and from observed anonymous requests against every collection on 2026-08-01. The\n  derive-authentication.py pass produced nothing because the derived OpenAPI declares\n  no `securitySchemes` — that absence is the accurate finding, not a gap: the public\n  read surface genuinely requires no credential.\nsummary:\n  types: [none, http]\n  anonymous_read: true\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\napi: kallyope:content-api\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n\
  \    Every GET collection and item route described in\n    openapi/kallyope-content-api-openapi.yml returned HTTP 200 with real JSON and no\n    credential of any kind. There is no API key, no signup, no token issuance and no\n    per-consumer identity on this surface.\n  applies_to: all read operations\n  sources: [openapi/kallyope-content-api-openapi.yml]\n  evidence:\n    observed: '2026-08-01'\n    example: GET https://kallyope.com/wp-json/wp/v2/document?per_page=1 -> 200\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords, advertised verbatim by the route index\n    `authentication` block. Credentials are minted per WordPress user in the site admin\n    and presented as HTTP Basic. This is the write/administrative path — it is not\n    offered to third parties and no self-service registration exists.\n  authorization_endpoint: https://kallyope.com/wp-admin/authorize-application.php\n  audience: internal WordPress users\
  \ only\n  sources: [https://kallyope.com/wp-json/]\n- name: cookie-nonce\n  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description: >-\n    The stock WordPress logged-in cookie plus an `X-WP-Nonce` header, used by the block\n    editor and admin JavaScript. Advertised indirectly by the\n    `Access-Control-Allow-Headers: Authorization, X-WP-Nonce, ...` response header\n    observed on every route. Browser-session only; not a third-party integration path.\n  sources: [https://kallyope.com/wp-json/wp/v2/document]\nobservations:\n- Anonymous writes are not possible - POST/PUT/PATCH/DELETE are registered on these\n  collections but every mutating endpoint is capability-gated behind the two schemes above.\n- 'GET /wp/v2/settings returned 401 {\"code\":\"rest_forbidden\",\"data\":{\"status\":401}} anonymously,\n  confirming the capability gate is enforced rather than merely documented.'\n- No OAuth 2.0, OpenID Connect or mTLS surface exists; /.well-known/openid-configuration\n\
  \  and /.well-known/oauth-authorization-server both returned 404 on kallyope.com.\n- No rate limiting, quota or per-consumer throttling headers were observed on any response.\nscopes: none\nscopes_note: >-\n  No OAuth scope surface exists. WordPress authorizes by user capability\n  (read/edit_posts/manage_options), not by scope, so scopes/ is deliberately absent\n  rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/authentication/kallyope-authentication.yml
summary_line: none/http · 3 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Drug Discovery
- Neuroscience
- Gut-Brain Axis
- Migraine
- Metabolic Disease
- Clinical Trials
- Content
---
