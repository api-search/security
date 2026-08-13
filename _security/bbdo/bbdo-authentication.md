---
api_key_in: []
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Bbdo Authentication
name_suffix: Authentication
oauth_flows: []
overview: BBDO Worldwide secures its APIs with none and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BBDO Worldwide
provider_slug: bbdo
scheme_count: 3
schemes:
- description: Read operations on public content are open. GET on wp/v2/work, wp/v2/news, wp/v2/posts, wp/v2/pages, wp/v2/categories, wp/v2/users and the oembed endpoints all returned HTTP 200 with no credentials.
  name: anonymous
  sources:
  - discovery/bbdo-wp-json-root.json
  type: none
  verified:
  - status: 200
    url: https://bbdo.com/wp-json/wp/v2/work?per_page=1
  - status: 200
    url: https://bbdo.com/wp-json/wp/v2/news?per_page=1
- authorization_endpoint: https://bbdo.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, advertised in the REST root's `authentication` object. Credentials are issued per-user from the site's own admin at the authorization endpoint below and presented as HTTP Basic. This is an operator/editor credential path, not a developer program — BBDO offers no self-service registration.
  name: application-passwords
  scheme: basic
  sources:
  - discovery/bbdo-wp-json-root.json
  type: http
- description: The standard WordPress logged-in cookie plus nonce path. Inferred from the Access-Control-Allow-Headers response header on wp/v2 collections, which advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`. Only usable from an authenticated browser session.
  in: header
  name: cookie-and-nonce
  parameter: X-WP-Nonce
  sources:
  - observed response header on https://bbdo.com/wp-json/wp/v2/work
  type: apiKey
slug: bbdo-authentication
source_filename: bbdo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://bbdo.com/wp-json/ (authentication block) + observed responses\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nnote: >-\n  Derived from the authentication block BBDO's own WordPress REST API root\n  advertises, plus observed anonymous behaviour. BBDO publishes no auth\n  documentation of its own; the model below is the WordPress platform default as\n  configured on bbdo.com. There is no OpenAPI securitySchemes block to read\n  because BBDO publishes no OpenAPI.\nsummary:\n  types:\n    - none\n    - http\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\nschemes:\n  - name: anonymous\n    type: none\n    description: >-\n      Read operations on public content are open. GET on wp/v2/work, wp/v2/news,\n      wp/v2/posts, wp/v2/pages, wp/v2/categories, wp/v2/users and the oembed\n      endpoints all returned HTTP 200 with no credentials.\n    verified:\n      - {url: 'https://bbdo.com/wp-json/wp/v2/work?per_page=1',\
  \ status: 200}\n      - {url: 'https://bbdo.com/wp-json/wp/v2/news?per_page=1', status: 200}\n    sources: [discovery/bbdo-wp-json-root.json]\n  - name: application-passwords\n    type: http\n    scheme: basic\n    description: >-\n      WordPress Application Passwords, advertised in the REST root's\n      `authentication` object. Credentials are issued per-user from the site's\n      own admin at the authorization endpoint below and presented as HTTP Basic.\n      This is an operator/editor credential path, not a developer program — BBDO\n      offers no self-service registration.\n    authorization_endpoint: https://bbdo.com/wp-admin/authorize-application.php\n    sources: [discovery/bbdo-wp-json-root.json]\n  - name: cookie-and-nonce\n    type: apiKey\n    in: header\n    parameter: X-WP-Nonce\n    description: >-\n      The standard WordPress logged-in cookie plus nonce path. Inferred from the\n      Access-Control-Allow-Headers response header on wp/v2 collections, which\n      advertises\
  \ `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5,\n      Content-Type`. Only usable from an authenticated browser session.\n    sources: ['observed response header on https://bbdo.com/wp-json/wp/v2/work']\nwrite_operations:\n  authenticated: true\n  evidence:\n    url: https://bbdo.com/wp-json/wp/v2/work\n    method: POST\n    status: 401\n    body: '{\"code\":\"rest_cannot_create\",\"message\":\"Sorry, you are not allowed to create posts as this user.\",\"data\":{\"status\":401}}'\noauth: false\noauth_note: >-\n  No OAuth 2.0 or OpenID Connect surface. /.well-known/oauth-authorization-server\n  and /.well-known/openid-configuration both returned 404, and no oauth\n  namespace is registered in the REST root. scopes/ is therefore not applicable\n  and no OAuthScopes artifact is written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bbdo/refs/heads/main/authentication/bbdo-authentication.yml
summary_line: none/http · 3 schemes
tags:
- Advertising
- Marketing
- Creative
- Agency
- Agency Network
- Holding Company Subsidiary
- Brand Strategy
- Media
- Content
- WordPress
---
