---
api_key_in: []
api_specs:
- filename: interpublic-wp-v2-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress Wp/v2 API
  slug: wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-wp-v2-api-openapi.yml
- filename: interpublic-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress Abilities API
  slug: wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-wp-abilities-v1-api-openapi.yml
- filename: interpublic-oembed-1-0-api-openapi.yml
  format: yaml
  label: Interpublic Group oEmbed API
  slug: oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-oembed-1-0-api-openapi.yml
- filename: interpublic-root-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress REST Index API
  slug: root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-root-api-openapi.yml
auth_types:
- none
- cookie
description: ''
kind: authentication
layout: security
method: probed
name: Interpublic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interpublic Group secures its APIs with none and cookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interpublic Group
provider_slug: interpublic
scheme_count: 2
schemes:
- applies_to:
  - GET /wp-json/
  - GET /wp-json/wp/v2/posts
  - GET /wp-json/wp/v2/pages
  - GET /wp-json/wp/v2/media
  - GET /wp-json/wp/v2/categories
  - GET /wp-json/wp/v2/tags
  - GET /wp-json/wp/v2/types
  - GET /wp-json/wp/v2/search
  - GET /wp-json/oembed/1.0/embed
  evidence: observed HTTP 200 without credentials, 2026-08-12
  name: anonymous
  type: none
- applies_to:
  - GET /wp-json/wp/v2/users
  - GET /wp-json/wp/v2/settings
  - GET /wp-json/wp-abilities/v1/abilities
  - GET /wp-json/wp-abilities/v1/categories
  - all POST/PUT/PATCH/DELETE operations
  description: WordPress core's built-in scheme - a logged-in session cookie plus an `X-WP-Nonce` request header. Documented in the WordPress REST API Handbook. Intended for first-party JavaScript inside wp-admin; not a credential a third party can be issued.
  docs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/
  evidence: observed HTTP 401 without credentials with body {"code":"rest_forbidden","message":"Sorry, you are not allowed to do that.","data":{"status":401}} (settings, abilities) and {"code":"rest_user_cannot_view",...} (users), 2026-08-12
  in: header
  name: wordpress-cookie-nonce
  parameter: X-WP-Nonce
  type: cookie
slug: interpublic-authentication
source_filename: interpublic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live anonymous probes of https://interpublic.com/wp-json/* (2026-08-12) plus\n  the WordPress REST API Handbook authentication reference\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary:\n  types:\n    - none\n    - cookie\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The four specs in openapi/ declare no `securitySchemes`, and that is\n    faithful to the surface: WordPress core advertises no authentication\n    scheme in its route-discovery document. The live discovery document's\n    `authentication` array is empty ([]), meaning no authentication plugin is\n    registered on this install. Read access is anonymous; write access and\n    privileged reads are gated by the WordPress cookie + `X-WP-Nonce` scheme,\n    which is only obtainable from an authenticated wp-admin session and is\n    not usable by a third-party integrator. There is therefore no\n    machine-issued\
  \ credential a developer can obtain for this API.\nschemes:\n  - name: anonymous\n    type: none\n    applies_to:\n      - GET /wp-json/\n      - GET /wp-json/wp/v2/posts\n      - GET /wp-json/wp/v2/pages\n      - GET /wp-json/wp/v2/media\n      - GET /wp-json/wp/v2/categories\n      - GET /wp-json/wp/v2/tags\n      - GET /wp-json/wp/v2/types\n      - GET /wp-json/wp/v2/search\n      - GET /wp-json/oembed/1.0/embed\n    evidence: 'observed HTTP 200 without credentials, 2026-08-12'\n  - name: wordpress-cookie-nonce\n    type: cookie\n    description: >-\n      WordPress core's built-in scheme - a logged-in session cookie plus an\n      `X-WP-Nonce` request header. Documented in the WordPress REST API\n      Handbook. Intended for first-party JavaScript inside wp-admin; not a\n      credential a third party can be issued.\n    parameter: X-WP-Nonce\n    in: header\n    docs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\n    applies_to:\n      - GET /wp-json/wp/v2/users\n\
  \      - GET /wp-json/wp/v2/settings\n      - GET /wp-json/wp-abilities/v1/abilities\n      - GET /wp-json/wp-abilities/v1/categories\n      - all POST/PUT/PATCH/DELETE operations\n    evidence: >-\n      observed HTTP 401 without credentials with body\n      {\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do\n      that.\",\"data\":{\"status\":401}} (settings, abilities) and\n      {\"code\":\"rest_user_cannot_view\",...} (users), 2026-08-12\noauth:\n  present: false\n  evidence: >-\n    /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource both 301 away from the origin and\n    terminate on the Omnicom HTML homepage; no RFC 8414 or RFC 9728 metadata\n    is served on any Interpublic Group host. No `mcp` namespace is registered\n    in the route-discovery document either, so there is no OAuth 2.1 surface\n    of the kind other WordPress installs in this catalog expose.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/authentication/interpublic-authentication.yml
summary_line: none/cookie · 2 schemes
tags:
- Advertising
- Marketing
- Fortune 500
- Holding Company
- Media
- Content
- WordPress
- Newsroom
---
