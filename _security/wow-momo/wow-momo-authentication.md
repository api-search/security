---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: wow-momo-content-api-openapi.yml
  format: yaml
  label: WOW! Momo Content API
  slug: wow-momo-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wow-momo/refs/heads/main/openapi/_ae-authored/wow-momo-content-api-openapi.yml
auth_types:
- http
- apiKey
- opaque-application-credential
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Wow Momo Authentication
name_suffix: Authentication
oauth_flows: []
overview: WOW! Momo secures its APIs with http, apiKey, and opaque-application-credential across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WOW! Momo
provider_slug: wow-momo
scheme_count: 3
schemes:
- authorization_endpoint: https://www.wowmomo.com/wp-admin/authorize-application.php
  evidence: The /wp-json/ index declares authentication.application-passwords.endpoints.authorization verbatim as https://www.wowmomo.com/wp-admin/authorize-application.php.
  hosts:
  - https://www.wowmomo.com
  name: applicationPassword
  note: WordPress application passwords. Required for every write on the content surface. Issued only from inside wp-admin, so no third party can obtain one.
  scheme: basic
  sources:
  - openapi/wow-momo-content-api-discovery-original.json
  type: http
- evidence: 'Observed 2026-09-04 in the live response header access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type.'
  hosts:
  - https://www.wowmomo.com
  in: header
  name: wpNonce
  name_header: X-WP-Nonce
  note: Cookie-session nonce; usable only from a browser already logged in to wp-admin.
  type: apiKey
- evidence: Every anonymous request to api.wowmomo.com on 2026-09-04 — including the control path /.well-known/wow-momo-negative-control-9f2c41d7, which cannot exist — returned HTTP 200 with the identical body {"data":null,"message":"NO_AUTH","messageType":"FAILED"} from an Express service behind an AWS Application Load Balancer. Only GET /health answers differently, returning "OK".
  hosts:
  - https://api.wowmomo.com
  name: wowMomoAppCredential
  note: The credential scheme is not documented anywhere public. The gate returns 200 rather than 401, so even the failure mode is undiscoverable by status code alone; the message name (NO_AUTH) is the only signal. Issuance path, credential format, header name and scope model are all unobservable without a credential. Recorded as gated, not guessed.
  type: opaque-application-credential
slug: wow-momo-authentication
source_filename: wow-momo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://www.wowmomo.com/wp-json/ route-discovery document (HTTP 200, saved verbatim to\n  openapi/wow-momo-content-api-discovery-original.json) plus live anonymous probes of\n  www.wowmomo.com and api.wowmomo.com on 2026-09-04\ndocs: null\nnote: >-\n  WOW! Momo publishes no authentication documentation of any kind. This profile is read from the live\n  route-discovery document's own `authentication` block, from response headers observed on the wire,\n  and from the bodies the hosts return anonymously. Nothing here is inferred from a vendor default.\nsummary:\n  types:\n  - http\n  - apiKey\n  - opaque-application-credential\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  hosts:\n  - https://www.wowmomo.com\n  authorization_endpoint: https://www.wowmomo.com/wp-admin/authorize-application.php\n  evidence: >-\n    The /wp-json/ index declares authentication.application-passwords.endpoints.authorization\
  \ verbatim\n    as https://www.wowmomo.com/wp-admin/authorize-application.php.\n  sources:\n  - openapi/wow-momo-content-api-discovery-original.json\n  note: >-\n    WordPress application passwords. Required for every write on the content surface. Issued only from\n    inside wp-admin, so no third party can obtain one.\n- name: wpNonce\n  type: apiKey\n  in: header\n  name_header: X-WP-Nonce\n  hosts:\n  - https://www.wowmomo.com\n  evidence: >-\n    Observed 2026-09-04 in the live response header access-control-allow-headers: Authorization,\n    X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type.\n  note: Cookie-session nonce; usable only from a browser already logged in to wp-admin.\n- name: wowMomoAppCredential\n  type: opaque-application-credential\n  hosts:\n  - https://api.wowmomo.com\n  evidence: >-\n    Every anonymous request to api.wowmomo.com on 2026-09-04 — including the control path\n    /.well-known/wow-momo-negative-control-9f2c41d7, which cannot exist — returned\
  \ HTTP 200 with the\n    identical body {\"data\":null,\"message\":\"NO_AUTH\",\"messageType\":\"FAILED\"} from an Express service\n    behind an AWS Application Load Balancer. Only GET /health answers differently, returning \"OK\".\n  note: >-\n    The credential scheme is not documented anywhere public. The gate returns 200 rather than 401, so\n    even the failure mode is undiscoverable by status code alone; the message name (NO_AUTH) is the only\n    signal. Issuance path, credential format, header name and scope model are all unobservable without a\n    credential. Recorded as gated, not guessed.\nanonymous_read:\n  available: true\n  hosts:\n  - https://www.wowmomo.com/wp-json\n  note: >-\n    The wp/v2 content collections read with no credential at all. pages, media, categories, tags, users,\n    types, taxonomies, statuses, search, comments and blocks all returned HTTP 200 anonymously on\n    2026-09-04, each with `Allow: GET`, as did /oembed/1.0/embed and /yoast/v1/get_head.\n\
  \  gated_anonymously:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_cannot_view_plugins\n  - path: /wp/v2/themes\n    status: 401\n    code: rest_cannot_view_themes\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n  - path: /contact-form-7/v1/contact-forms\n    status: 403\n    code: wpcf7_forbidden\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wow-momo/refs/heads/main/authentication/wow-momo-authentication.yml
summary_line: http/apiKey/opaque-application-credential · 3 schemes
tags:
- Company
- Restaurants
- Food and Beverage
- Quick Service Restaurant
- Retail
- Hospitality
- Consumer
- Franchising
- Content
- WordPress
- oEmbed
- India
- Kolkata
---
