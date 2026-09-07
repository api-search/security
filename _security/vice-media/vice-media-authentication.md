---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: vice-media-wp-rest-openapi.yml
  format: yaml
  label: VICE WordPress REST API
  slug: vice-media-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/openapi/_ae-authored/vice-media-wp-rest-openapi.yml
- filename: vice-media-video-wp-rest-openapi.yml
  format: yaml
  label: VICE Video WordPress REST API
  slug: vice-media-video-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/openapi/_ae-authored/vice-media-video-wp-rest-openapi.yml
auth_types:
- http
- apiKey
- opaque-client-credential
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Vice Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vice Media secures its APIs with http, apiKey, and opaque-client-credential across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vice Media
provider_slug: vice-media
scheme_count: 3
schemes:
- authorization_endpoint: https://www.vice.com/wp-admin/authorize-application.php
  evidence: The /wp-json/ index declares authentication.application-passwords.endpoints.authorization verbatim; video.vice.com declares the same at its own /wp-admin/authorize-application.php.
  hosts:
  - https://www.vice.com
  - https://video.vice.com
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/vice-media-wp-rest-discovery-original.json
  type: http
- evidence: 'Observed 2026-09-04 in the live response header access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type.'
  hosts:
  - https://www.vice.com
  - https://video.vice.com
  in: header
  name: wpNonce
  name_header: X-WP-Nonce
  note: Cookie-session nonce; only usable from a browser session already logged into wp-admin.
  type: apiKey
- evidence: 'Every anonymous request to api.vice.com — including the control path /vice-media-negative-control-7f3ab91c, which cannot exist — returned HTTP 401 {"message":"No client found attached to request","code":"invalid_req_client","status":401} from a service identifying itself as x-app-version: api-auth 1.13.2. The gate sets SB_SID / AUTH_SID / C_U cookies on Domain=vice.com.'
  hosts:
  - https://api.vice.com
  name: viceApiClient
  note: The credential scheme is not documented anywhere public. The error name (invalid_req_client) and the session cookies indicate a registered-client model, but the issuance path, token format and scope model are all unobservable without a credential. Recorded as gated, not guessed.
  type: opaque-client-credential
slug: vice-media-authentication
source_filename: vice-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.vice.com/wp-json/ (route-discovery document, HTTP 200) plus live anonymous probes\n  of api.vice.com\ndocs: null\nnote: Vice Media publishes no authentication documentation of any kind. This profile is read from the\n  live route-discovery document's own `authentication` block, from response headers observed on the wire,\n  and from the HTTP 401 bodies the hosts return anonymously.\nsummary:\n  types:\n  - http\n  - apiKey\n  - opaque-client-credential\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  hosts:\n  - https://www.vice.com\n  - https://video.vice.com\n  authorization_endpoint: https://www.vice.com/wp-admin/authorize-application.php\n  evidence: The /wp-json/ index declares authentication.application-passwords.endpoints.authorization\n    verbatim; video.vice.com declares the same at its own /wp-admin/authorize-application.php.\n  sources:\n\
  \  - openapi/vice-media-wp-rest-discovery-original.json\n- name: wpNonce\n  type: apiKey\n  in: header\n  name_header: X-WP-Nonce\n  hosts:\n  - https://www.vice.com\n  - https://video.vice.com\n  evidence: 'Observed 2026-09-04 in the live response header access-control-allow-headers: Authorization,\n    X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type.'\n  note: Cookie-session nonce; only usable from a browser session already logged into wp-admin.\n- name: viceApiClient\n  type: opaque-client-credential\n  hosts:\n  - https://api.vice.com\n  evidence: 'Every anonymous request to api.vice.com — including the control path /vice-media-negative-control-7f3ab91c,\n    which cannot exist — returned HTTP 401 {\"message\":\"No client found attached to request\",\"code\":\"invalid_req_client\",\"status\":401}\n    from a service identifying itself as x-app-version: api-auth 1.13.2. The gate sets SB_SID / AUTH_SID\n    / C_U cookies on Domain=vice.com.'\n  note: The credential scheme\
  \ is not documented anywhere public. The error name (invalid_req_client) and\n    the session cookies indicate a registered-client model, but the issuance path, token format and scope\n    model are all unobservable without a credential. Recorded as gated, not guessed.\nanonymous_read:\n  available: true\n  hosts:\n  - https://www.vice.com/wp-json\n  - https://video.vice.com/wp-json\n  note: 'The wp/v2 content collections read with no credential at all: posts, pages, media, search, types,\n    statuses, taxonomies, and the vice_section / profile / sp_product custom post types all returned HTTP\n    200 anonymously on 2026-09-04.'\n  gated_anonymously:\n  - /wp/v2/users\n  - /wp/v2/settings\n  - /wp/v2/comments\n  - /wp/v2/block-types\n  - /wp-abilities/v1/abilities\n  - /wp-abilities/v1/categories\n  - /byline-manager/v1/authors\n  - /wp-curate/v1/posts\n  - /elasticpress/v1/facets/taxonomies\n  - /vip/v1/sites\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/authentication/vice-media-authentication.yml
summary_line: http/apiKey/opaque-client-credential · 3 schemes
tags:
- Company
- Media
- Publishing
- News
- Digital Media
- Content
- Video
- Entertainment
- WordPress
- Syndication
- oEmbed
- Brooklyn
---
