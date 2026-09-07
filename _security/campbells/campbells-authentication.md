---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'The Campbell''s read surface requires no authentication at all: every content and search endpoint returned 200 anonymously. There is no API key, no OAuth, no signup and no developer account — which means there is also no way for an outside developer to authenticate into the routes that do require a credential.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Campbells Authentication
name_suffix: Authentication
oauth_flows: []
overview: Campbell's declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Campbell's
provider_slug: campbells
scheme_count: 3
schemes:
- applies_to: All read routes exercised — /wp/v2/recipe, /wp/v2/product, /wp/v2/csc_faq, /wp/v2/external_product, every csc_* taxonomy, /wp/v2/types, /yrsc-search/v1/query, /yrsc-search/v1/autocomplete, /yrsc-search/v1/featured-collections.
  evidence: GET https://www.campbells.com/wp-json/wp/v2/recipe?per_page=1 returned 200 with no Authorization header.
  id: none
  type: none
- applies_to: Browser-session writes from the site's own front end.
  evidence: access-control-allow-headers on the OPTIONS preflight names "Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type", and access-control-allow-credentials is true.
  header: X-WP-Nonce
  id: wordpress-cookie-nonce
  note: Issued to a logged-in WordPress session only.
  obtainable: false
  type: cookie
- applies_to: Programmatic writes as a WordPress user.
  evidence: The route descriptor registers /wp/v2/users/(?P<user_id>(?:[\d]+|me))/application-passwords and its /introspect sibling.
  id: wordpress-application-passwords
  note: Requires an existing WordPress user account on campbells.com. Recorded because the platform registers it, not because Campbell's offers it.
  obtainable: false
  scheme: basic
  type: http
slug: campbells-authentication
source_filename: campbells-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Campbell's\nproviderId: campbells\ngenerated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live probes of https://www.campbells.com/wp-json/ and reading of the\n  provider-served route descriptor in discovery/campbells-wp-v2-routes.json,\n  2026-09-05. Campbell's publishes no authentication documentation.\ndescription: >-\n  The Campbell's read surface requires no authentication at all: every content\n  and search endpoint returned 200 anonymously. There is no API key, no OAuth,\n  no signup and no developer account — which means there is also no way for an\n  outside developer to authenticate into the routes that do require a\n  credential.\nsummary:\n  public_read: true\n  credential_obtainable_by_developers: false\n  signup_url: null\n  key_prefixes: []\nschemes:\n  - id: none\n    type: none\n    applies_to: >-\n      All read routes exercised — /wp/v2/recipe, /wp/v2/product, /wp/v2/csc_faq,\n\
  \      /wp/v2/external_product, every csc_* taxonomy, /wp/v2/types,\n      /yrsc-search/v1/query, /yrsc-search/v1/autocomplete,\n      /yrsc-search/v1/featured-collections.\n    evidence: >-\n      GET https://www.campbells.com/wp-json/wp/v2/recipe?per_page=1 returned 200\n      with no Authorization header.\n  - id: wordpress-cookie-nonce\n    type: cookie\n    header: X-WP-Nonce\n    applies_to: Browser-session writes from the site's own front end.\n    evidence: >-\n      access-control-allow-headers on the OPTIONS preflight names\n      \"Authorization, X-WP-Nonce, Content-Disposition, Content-MD5,\n      Content-Type\", and access-control-allow-credentials is true.\n    obtainable: false\n    note: Issued to a logged-in WordPress session only.\n  - id: wordpress-application-passwords\n    type: http\n    scheme: basic\n    applies_to: Programmatic writes as a WordPress user.\n    evidence: >-\n      The route descriptor registers\n      /wp/v2/users/(?P<user_id>(?:[\\d]+|me))/application-passwords\
  \ and its\n      /introspect sibling.\n    obtainable: false\n    note: >-\n      Requires an existing WordPress user account on campbells.com. Recorded\n      because the platform registers it, not because Campbell's offers it.\ndenied_anonymously:\n  - route: /wp/v2/settings\n    http_status: 401\n    code: rest_forbidden\n  - route: /wp/v2/plugins\n    http_status: 401\n    code: rest_cannot_view_plugins\noauth:\n  supported: false\n  detail: >-\n    No oauth2 or openIdConnect scheme is registered. /.well-known/openid-configuration\n    and /.well-known/oauth-authorization-server both 404 on every host — see\n    well-known/campbells-well-known.yml. No scopes/ artifact is emitted, because\n    there is no scope surface to describe.\nmtls:\n  supported: false\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbells/refs/heads/main/authentication/campbells-authentication.yml
summary_line: 3 schemes
tags:
- Food
- Consumer Packaged Goods
- Recipes
- Brands
- Nutrition
- Content
- Product Catalog
- WordPress
---
