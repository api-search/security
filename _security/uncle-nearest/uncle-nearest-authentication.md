---
api_key_in: []
api_specs:
- filename: uncle-nearest-events-calendar-v1-openapi.json
  format: json
  label: Uncle Nearest Events Calendar REST API (tribe/events/v1)
  slug: uncle-nearest-events-calendar-rest-api-tribeeventsv1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncle-nearest/refs/heads/main/openapi/uncle-nearest-events-calendar-v1-openapi.json
- filename: uncle-nearest-tec-v1-openapi.json
  format: json
  label: Uncle Nearest Events Calendar REST API (tec/v1)
  slug: uncle-nearest-events-calendar-rest-api-tecv1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncle-nearest/refs/heads/main/openapi/uncle-nearest-tec-v1-openapi.json
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
method: derived
name: Uncle Nearest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncle Nearest secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uncle Nearest
provider_slug: uncle-nearest
scheme_count: 2
schemes:
- name: BasicAuth
  note: Declared in components.securitySchemes but not applied to any individual operation via a security[] requirement, so the spec does not say which operations need it. In practice it is the WordPress application-password mechanism, used only for writes.
  scheme: basic
  sources:
  - openapi/uncle-nearest-tec-v1-openapi.json
  type: http
- name: none
  note: 'The tribe/events/v1 document declares no securitySchemes at all, and the WordPress route index reports "authentication": []. GET operations over published content returned 200 anonymously on 2026-08-02.'
  sources:
  - openapi/uncle-nearest-events-calendar-v1-openapi.json
  - openapi/uncle-nearest-tec-v1-openapi.json
  type: none
slug: uncle-nearest-authentication
source_filename: uncle-nearest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: >-\n  openapi/uncle-nearest-tec-v1-openapi.json, openapi/uncle-nearest-events-calendar-v1-openapi.json, and the live\n  WordPress REST route index at https://unclenearest.com/wp-json/ (fetched 2026-08-02, \"authentication\": [])\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndocs_note: >-\n  Upstream WordPress documentation. Uncle Nearest publishes no authentication documentation of its own — there is no\n  developer portal, no API key issuance and no signup flow.\nsummary:\n  types:\n  - http\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_reads: true\n  credential_issuance: none-public\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/uncle-nearest-tec-v1-openapi.json\n  note: >-\n    Declared in components.securitySchemes but not applied to any individual operation via a security[] requirement,\n    so the spec does not say which operations\
  \ need it. In practice it is the WordPress application-password\n    mechanism, used only for writes.\n- name: none\n  type: none\n  sources:\n  - openapi/uncle-nearest-events-calendar-v1-openapi.json\n  - openapi/uncle-nearest-tec-v1-openapi.json\n  note: >-\n    The tribe/events/v1 document declares no securitySchemes at all, and the WordPress route index reports\n    \"authentication\": []. GET operations over published content returned 200 anonymously on 2026-08-02.\nmechanisms:\n- name: Anonymous read\n  applies_to: All GET operations over published content\n  credential: none\n- name: WordPress application password over HTTP Basic\n  applies_to: POST / PUT / DELETE on events, venues, organizers\n  credential: WordPress user plus an application password\n  issuance: Requires a WordPress account on unclenearest.com; not available to the public.\n- name: Cookie plus X-WP-Nonce\n  applies_to: Same-origin browser requests from a logged-in admin\n  credential: WordPress session cookie\
  \ plus a nonce in the X-WP-Nonce header\n  note: >-\n    The route index advertises X-WP-Nonce and Authorization in its Access-Control-Allow-Headers, confirming both paths\n    are wired.\nnot_present:\n- oauth2\n- openIdConnect\n- mutualTLS\n- apiKey\n- jwt\ngaps:\n- No per-operation security[] requirements in either spec, so required privileges must be inferred from the 401/403 responses.\n- No public credential issuance — writes are effectively unavailable to third parties.\n- No scopes surface; scopes/ is intentionally not emitted for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncle-nearest/refs/heads/main/authentication/uncle-nearest-authentication.yml
summary_line: http/none · 2 schemes
tags:
- Company
- whiskey
- spirits
- beverage-alcohol
- consumer-packaged-goods
- distillery
- hospitality
- events
- tennessee
- wordpress
---
