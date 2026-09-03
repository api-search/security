---
api_key_in: []
api_specs:
- filename: alliance-resource-partners-content-openapi.yml
  format: yaml
  label: Alliance Resource Partners Content API
  slug: alliance-resource-partners-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-resource-partners/refs/heads/main/openapi/_original/alliance-resource-partners-content-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Alliance Resource Partners Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alliance Resource Partners secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alliance Resource Partners
provider_slug: alliance-resource-partners
scheme_count: 2
schemes:
- description: Every GET operation in openapi/ was verified to return HTTP 200 with no credential on 2026-09-01. The entire published read surface of the ARLP Content API is anonymous. No API key, no bearer token, no OAuth, no registration and no rate-limit key.
  name: anonymous
  sources:
  - https://www.arlp.com/wp-json/
  type: none
- authorization_endpoint: https://www.arlp.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, declared by the site's own discovery document at https://www.arlp.com/wp-json/ under `authentication.application-passwords`. Credentials are issued per WordPress user from the wp-admin authorize-application screen and sent as HTTP Basic. This gates the write surface and the administrative namespaces; it is a WordPress account credential, not a developer-program API key, and ARLP does not issue one to third parties.
  name: application-passwords
  scheme: basic
  sources:
  - https://www.arlp.com/wp-json/
  type: http
slug: alliance-resource-partners-authentication
source_filename: alliance-resource-partners-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://www.arlp.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nnote: >-\n  Alliance Resource Partners publishes no authentication documentation, because it publishes no developer\n  program. This profile is read from the live WordPress REST API discovery document served by www.arlp.com,\n  which declares its own supported authentication scheme, plus live anonymous probes of every route.\nsummary:\n  types: [none, http]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  gated_write: true\nschemes:\n  - name: anonymous\n    type: none\n    description: >-\n      Every GET operation in openapi/ was verified to return HTTP 200 with no credential on 2026-09-01. The\n      entire published read surface of the ARLP Content API is anonymous. No API key, no bearer token, no\n      OAuth, no registration and no rate-limit key.\n    sources: [https://www.arlp.com/wp-json/]\n\
  \  - name: application-passwords\n    type: http\n    scheme: basic\n    description: >-\n      WordPress Application Passwords, declared by the site's own discovery document at\n      https://www.arlp.com/wp-json/ under `authentication.application-passwords`. Credentials are issued\n      per WordPress user from the wp-admin authorize-application screen and sent as HTTP Basic. This gates\n      the write surface and the administrative namespaces; it is a WordPress account credential, not a\n      developer-program API key, and ARLP does not issue one to third parties.\n    authorization_endpoint: https://www.arlp.com/wp-admin/authorize-application.php\n    sources: [https://www.arlp.com/wp-json/]\ngated_surface_evidence:\n  - url: https://www.arlp.com/wp-json/wp/v2/settings\n    status: 401\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n  - url: https://www.arlp.com/wp-json/wp-abilities/v1/abilities\n    status:\
  \ 401\n    note: The WordPress Abilities API namespace is registered but requires authentication.\n  - url: https://www.arlp.com/wp-json/wp/v2/block-types\n    status: 401\ncors:\n  access_control_allow_headers: [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type]\n  access_control_expose_headers: [X-WP-Total, X-WP-TotalPages, Link]\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-resource-partners/refs/heads/main/authentication/alliance-resource-partners-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Coal
- Mining
- Energy
- Royalties
- Natural Resources
- Content
- Corporate
---
