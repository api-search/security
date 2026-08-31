---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Provivi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Provivi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Provivi
provider_slug: provivi
scheme_count: 2
schemes:
- applies_to: read
  description: GraphQL introspection and read queries on https://api.provivi.com/admin/api both succeed with no Authorization header, no cookie and no API key. Verified 2026-08-26 - a full introspection query returned HTTP 200 with 199 types, and `{ _allProductsMeta { count } }` returned live content counts.
  evidence:
    http_status: 200
    url: https://api.provivi.com/admin/api
    verified: '2026-08-26'
  in: n/a
  name: none
  type: anonymous
- applies_to: write/admin
  description: 'KeystoneJS 5 session authentication. The schema declares `authenticatedUser`, `authenticateUserWithPassword`, `unauthenticateUser` and a User list, which is the standard Keystone session model. Querying `{ authenticatedUser { id } }` anonymously returns null, confirming no session is established for an anonymous caller. Whether the 122 declared mutation fields are access-controlled was NOT tested: this pipeline never executes write operations against a provider.'
  evidence:
    http_status: 200
    url: https://api.provivi.com/admin/api
    verified: '2026-08-26'
  in: cookie
  name: keystone-session
  type: cookie
slug: provivi-authentication
source_filename: provivi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://api.provivi.com/admin/api\nnote: >-\n  Provivi publishes no authentication documentation, because it publishes no developer program. This\n  profile records the auth behaviour actually observed against the live endpoint. No credential of any\n  kind was used, and no write operation was attempted.\nschemes:\n- name: none\n  type: anonymous\n  in: n/a\n  applies_to: read\n  description: >-\n    GraphQL introspection and read queries on https://api.provivi.com/admin/api both succeed with no\n    Authorization header, no cookie and no API key. Verified 2026-08-26 - a full introspection query\n    returned HTTP 200 with 199 types, and `{ _allProductsMeta { count } }` returned live content counts.\n  evidence:\n    url: https://api.provivi.com/admin/api\n    http_status: 200\n    verified: '2026-08-26'\n- name: keystone-session\n  type: cookie\n  in: cookie\n  applies_to: write/admin\n  description: >-\n    KeystoneJS 5 session\
  \ authentication. The schema declares `authenticatedUser`, `authenticateUserWithPassword`,\n    `unauthenticateUser` and a User list, which is the standard Keystone session model. Querying\n    `{ authenticatedUser { id } }` anonymously returns null, confirming no session is established for an\n    anonymous caller. Whether the 122 declared mutation fields are access-controlled was NOT tested:\n    this pipeline never executes write operations against a provider.\n  evidence:\n    url: https://api.provivi.com/admin/api\n    http_status: 200\n    verified: '2026-08-26'\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\ndocs: null\nobservations:\n- >-\n  Access-Control-Allow-Origin is `*` with Access-Control-Allow-Credentials `true` on the GraphQL endpoint.\n- >-\n  Both POST and GET carry queries; GET https://api.provivi.com/admin/api?query={__typename} returned 200.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provivi/refs/heads/main/authentication/provivi-authentication.yml
summary_line: 2 schemes
tags:
- Agriculture
- agtech
- biotechnology
- crop-protection
- pheromones
- sustainability
- content-management
- graphql
---
