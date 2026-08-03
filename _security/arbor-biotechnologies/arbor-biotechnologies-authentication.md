---
api_key_in: []
api_specs:
- filename: arbor-biotechnologies-content-openapi.yml
  format: yaml
  label: Arbor Biotechnologies Content API (WordPress REST)
  slug: arbor-biotechnologies-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbor-biotechnologies/refs/heads/main/openapi/arbor-biotechnologies-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arbor Biotechnologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arbor Biotechnologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arbor Biotechnologies
provider_slug: arbor-biotechnologies
scheme_count: 1
schemes:
- applies_to: write and administrative routes
  description: WordPress application passwords — a WordPress username plus a generated application password sent as HTTP Basic. The platform advertises the capability, with the authorization endpoint at https://arbor.bio/wp-admin/authorize-application.php. It applies only to write and administrative routes, none of which are in the OpenAPI. Arbor issues no public credentials, so this scheme is declared but unreachable for third parties.
  name: applicationPassword
  reachable_by_third_parties: false
  rfc: RFC 7617
  scheme: basic
  sources:
  - openapi/arbor-biotechnologies-content-openapi.yml
  - https://arbor.bio/wp-json
  type: http
slug: arbor-biotechnologies-authentication
source_filename: arbor-biotechnologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: >-\n  openapi/arbor-biotechnologies-content-openapi.yml, plus the authentication block of the live\n  route index at https://arbor.bio/wp-json and anonymous probes run on 2026-07-31\nnote: >-\n  Arbor Biotechnologies publishes no authentication documentation — there is no developer\n  portal, no signup and no docs page to search, so this artifact stays derived. The entire\n  publicly reachable surface is anonymous: no key is issued and the one declared scheme is\n  closed to third parties in practice.\nsummary:\n  types:\n  - http\n  anonymous_read: true\n  credentials_issued_publicly: false\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\n  signup_url: null\n  developer_portal: null\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  rfc: RFC 7617\n  description: >-\n    WordPress application passwords — a WordPress username plus a generated application\n    password sent as HTTP Basic.\
  \ The platform advertises the capability, with the authorization\n    endpoint at https://arbor.bio/wp-admin/authorize-application.php. It applies only to write\n    and administrative routes, none of which are in the OpenAPI. Arbor issues no public\n    credentials, so this scheme is declared but unreachable for third parties.\n  applies_to: write and administrative routes\n  reachable_by_third_parties: false\n  sources:\n  - openapi/arbor-biotechnologies-content-openapi.yml\n  - https://arbor.bio/wp-json\nanonymous_access:\n  applies_to: every operation in openapi/arbor-biotechnologies-content-openapi.yml\n  verified: '2026-07-31'\n  detail: >-\n    Each read operation was probed with no credential of any kind and returned HTTP 200.\n    Note that the site fronts the API with a security layer that returns HTTP 406 to requests\n    carrying a non-browser User-Agent while still serving the correct JSON body; sending a\n    normal browser User-Agent yields a clean 200.\n  cors:\n    allow_headers:\
  \ [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type]\n    expose_headers: [X-WP-Total, X-WP-TotalPages, Link]\n    note: >-\n      Pagination headers are CORS-exposed, so a browser client can page the collections\n      cross-origin without a proxy.\ndenied_anonymously:\n  detail: >-\n    Routes declared in the live index that reject anonymous callers. They are deliberately\n    excluded from the OpenAPI rather than documented as available.\n  routes:\n  - {route: /wp/v2/users, status: 401, code: rest_user_cannot_view}\n  - {route: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {route: /wp/v2/plugins, status: 401, code: rest_cannot_view_plugins}\n  - {route: /wp/v2/themes, status: 401, code: rest_cannot_view_themes}\n  - {route: /wp/v2/block-types, status: 401, code: rest_block_type_cannot_view}\n  - {route: /wp/v2/menu-locations, status: 401, code: rest_cannot_view}\n  - {route: /wp/v2/font-collections, status: 401, code: rest_cannot_read}\n  - {route:\
  \ /wp/v2/widget-types, status: 401, code: rest_cannot_manage_widgets}\n  - {route: /wp-site-health/v1/tests/background-updates, status: 401, code: rest_forbidden}\n  - {route: /wp/v2/comments, status: 403, code: rest_comment_disabled}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbor-biotechnologies/refs/heads/main/authentication/arbor-biotechnologies-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Gene Editing
- CRISPR
- Genomic Medicine
- Life Sciences
- Drug Development
- Clinical Trials
- Neurology
- Rare Disease
- Healthcare
- Private Company
---
