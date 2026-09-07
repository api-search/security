---
anonymous_access: true
api_key_in: []
api_specs:
- filename: denbury-resources-pages-api-openapi.yml
  format: yaml
  label: Denbury Resources Pages API
  slug: denbury-resources-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-pages-api-openapi.yml
- filename: denbury-resources-media-api-openapi.yml
  format: yaml
  label: Denbury Resources Media API
  slug: denbury-resources-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-media-api-openapi.yml
- filename: denbury-resources-search-api-openapi.yml
  format: yaml
  label: Denbury Resources Search API
  slug: denbury-resources-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-search-api-openapi.yml
- filename: denbury-resources-discovery-api-openapi.yml
  format: yaml
  label: Denbury Resources Discovery API
  slug: denbury-resources-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-discovery-api-openapi.yml
- filename: denbury-resources-oembed-api-openapi.yml
  format: yaml
  label: Denbury Resources oEmbed API
  slug: denbury-resources-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-oembed-api-openapi.yml
auth_types: []
description: 'Denbury Inc. runs no developer program, issues no API keys, and documents no authentication. The WordPress core REST API behind www.denbury.com is the only machine-readable surface, and its public half needs no credentials at all: every route captured in openapi/ answers anonymously and advertises `Allow: GET`. The write half of the same routes exists but is refused anonymously.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Denbury Resources Authentication
name_suffix: Authentication
oauth_flows: []
overview: Denbury Resources declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Denbury Resources
provider_slug: denbury-resources
scheme_count: 3
schemes:
- applies_to: every operation in openapi/
  description: Anonymous read. No API key, token, cookie or nonce is required for any GET operation documented in openapi/.
  id: none
  method: probed
  type: none
- applies_to: write methods and context=edit (not documented in openapi/)
  description: WordPress application passwords, sent as HTTP Basic credentials. This is the only mechanism the server itself advertises, in the `authentication.application-passwords` block of the https://www.denbury.com/wp-json/ index, which names https://www.denbury.com/wp-admin/authorize-application.php as the authorization endpoint. It gates the write methods and the `edit` context, neither of which is part of the public surface described in openapi/. Credentials are issued only to Denbury site administrators.
  id: application-password
  method: searched
  scheme: basic
  source: https://www.denbury.com/wp-json/
  type: http
- applies_to: authenticated admin sessions only
  description: 'Cookie-authenticated browser sessions use an X-WP-Nonce header. The origin advertises it in `Access-Control-Allow-Headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`. It is a same-site admin mechanism, not an integration credential.'
  id: nonce
  in: header
  method: probed
  name: X-WP-Nonce
  source: response headers on https://www.denbury.com/wp-json/wp/v2/pages
  type: apiKey
slug: denbury-resources-authentication
source_filename: denbury-resources-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  https://www.denbury.com/wp-json/ (the server's own `authentication` block) plus live anonymous and\n  context=edit requests against the routes captured in openapi/\ndescription: >-\n  Denbury Inc. runs no developer program, issues no API keys, and documents no authentication.\n  The WordPress core REST API behind www.denbury.com is the only machine-readable surface, and its\n  public half needs no credentials at all: every route captured in openapi/ answers anonymously and\n  advertises `Allow: GET`. The write half of the same routes exists but is refused anonymously.\npublic_surface:\n  authentication_required: false\n  verified: '2026-09-06'\n  evidence: >-\n    GET https://www.denbury.com/wp-json/wp/v2/pages?per_page=1 returned HTTP 200 with\n    `Allow: GET` and X-WP-Total: 48, with no Authorization header sent.\n  scope: read-only\nschemes:\n- id: none\n  type: none\n  description: >-\n    Anonymous read. No API key,\
  \ token, cookie or nonce is required for any GET operation documented\n    in openapi/.\n  applies_to: every operation in openapi/\n  method: probed\n- id: application-password\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, sent as HTTP Basic credentials. This is the only mechanism the\n    server itself advertises, in the `authentication.application-passwords` block of the\n    https://www.denbury.com/wp-json/ index, which names\n    https://www.denbury.com/wp-admin/authorize-application.php as the authorization endpoint.\n    It gates the write methods and the `edit` context, neither of which is part of the public\n    surface described in openapi/. Credentials are issued only to Denbury site administrators.\n  applies_to: write methods and context=edit (not documented in openapi/)\n  method: searched\n  source: https://www.denbury.com/wp-json/\n- id: nonce\n  type: apiKey\n  in: header\n  name: X-WP-Nonce\n  description: >-\n    Cookie-authenticated\
  \ browser sessions use an X-WP-Nonce header. The origin advertises it in\n    `Access-Control-Allow-Headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5,\n    Content-Type`. It is a same-site admin mechanism, not an integration credential.\n  applies_to: authenticated admin sessions only\n  method: probed\n  source: response headers on https://www.denbury.com/wp-json/wp/v2/pages\ngated_surfaces:\n- surface: context=edit on any wp/v2 route\n  status: 401\n  body: '{\"code\":\"rest_forbidden_context\",\"message\":\"Sorry, you are not allowed to edit posts in this post type.\",\"data\":{\"status\":401}}'\n  note: Observed live on 2026-09-06. The extra fields in the `edit` context are not publicly readable.\n- surface: /wp-json/wp-abilities/v1/abilities\n  status: 401\n  body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n  note: >-\n    The WordPress Abilities API namespace is registered on this site but is\
  \ entirely auth-gated.\n    Its tool/ability catalogue cannot be introspected anonymously, so nothing about it is recorded\n    beyond its presence in the route index.\n- surface: /wp-json/wp/v2/users\n  status: 403\n  note: Author enumeration is blocked at the origin. No user records are publicly readable.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys_issued: false\nnotes:\n- Denbury publishes no authentication documentation because it publishes no developer program.\n- Nothing here was inferred; each row cites either the server's own index document or a live response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/authentication/denbury-resources-authentication.yml
summary_line: 3 schemes
tags:
- Acquired
- Carbon Capture
- CO2 EOR
- Energy
- Enhanced Oil Recovery
- ExxonMobil
- Oil and Gas
- Fortune 1000
- Content
- Carbon Sequestration
---
