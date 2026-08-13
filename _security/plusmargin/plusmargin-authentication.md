---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Plusmargin Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlusMargin declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: PlusMargin
provider_slug: plusmargin
scheme_count: 0
schemes: []
slug: plusmargin-authentication
source_filename: plusmargin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://plusmargin.com/wp-json — the `authentication` block of the live WordPress REST API\n  root discovery document, plus observed anonymous and gated responses\nprovider: PlusMargin\nproviderId: plusmargin\nsummary: >-\n  PlusMargin publishes no API program and therefore no authentication documentation. The only\n  authenticated surface reachable is the stock WordPress REST API on plusmargin.com, whose root\n  document advertises exactly one authentication method — WordPress Application Passwords (HTTP\n  Basic against an admin-issued application password). Read access to core content is anonymous;\n  everything write-scoped, and the Abilities API in full, requires credentials this pipeline does\n  not hold and did not attempt to obtain.\napis:\n- name: PlusMargin WordPress REST API\n  baseURL: https://plusmargin.com/wp-json\n  schemes:\n  - id: application-passwords\n    type: http\n    scheme: basic\n    in: header\n\
  \    header: Authorization\n    description: >-\n      WordPress Application Passwords. A logged-in WordPress user authorizes an application at\n      the endpoint below and receives a per-application password used as HTTP Basic credentials.\n      Advertised verbatim by the API's own root document.\n    authorizationEndpoint: https://plusmargin.com/wp-admin/authorize-application.php\n    source: https://plusmargin.com/wp-json\n    docs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\n  - id: cookie-nonce\n    type: apiKey\n    in: header\n    header: X-WP-Nonce\n    description: >-\n      Cookie + nonce authentication for same-origin browser requests. Not advertised in the\n      `authentication` block, but the API declares X-WP-Nonce in its\n      Access-Control-Allow-Headers response header, so the scheme is active on this install.\n    source: https://plusmargin.com/wp-json/wp/v2/posts\n    confidence: medium\n  anonymous_access:\n    readable: true\n \
  \   detail: >-\n      Core content collections are readable with no credentials — verified against\n      /wp-json/wp/v2/posts (200), /wp-json/wp/v2/types (200), /wp-json/wp/v2/categories (200)\n      and /wp-json/wp/v2/users (200).\n  gated:\n  - path: /wp-json/wp-abilities/v1/abilities\n    status: 401\n    error: rest_forbidden\n  - path: /wp-json/wp-abilities/v1/categories\n    status: 401\n    error: rest_forbidden\noauth2: false\nopenIdConnect: false\nmutualTLS: false\nnotes:\n- >-\n  No OAuth 2.0 or OpenID Connect surface exists: /.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource all 404.\n  No scopes artifact is emitted, because there are no scopes to enumerate.\n- >-\n  This is WordPress core's authentication model, not an authentication design PlusMargin\n  authored or documents. It is recorded because it is what an agent calling\n  plusmargin.com/wp-json actually encounters.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plusmargin/refs/heads/main/authentication/plusmargin-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketing
- Digital Marketing
- Consulting
- Advertising
- Customer Engagement
- Thailand
---
