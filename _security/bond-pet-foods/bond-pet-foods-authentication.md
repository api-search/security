---
api_key_in:
- header
api_specs:
- filename: bond-pet-foods-wc-store-v1-api-openapi.yml
  format: yaml
  label: Bond Pet Foods Wc/store/v1 API
  slug: bond-pet-foods-wc-store-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/openapi/bond-pet-foods-wc-store-v1-api-openapi.yml
- filename: bond-pet-foods-wp-v2-api-openapi.yml
  format: yaml
  label: Bond Pet Foods Wp/v2 API
  slug: bond-pet-foods-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/openapi/bond-pet-foods-wp-v2-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bond Pet Foods Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bond Pet Foods secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bond Pet Foods
provider_slug: bond-pet-foods
scheme_count: 3
schemes:
- description: WordPress cookie authentication nonce. Required for state-changing wp/v2 requests from a logged-in browser session.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/bond-pet-foods-content-openapi.json
  - openapi/bond-pet-foods-store-openapi.json
  type: apiKey
- description: WooCommerce Store API JWT session token identifying an anonymous cart. Returned in the Cart-Token response header.
  in: header
  name: cartToken
  parameter: Cart-Token
  sources:
  - openapi/bond-pet-foods-content-openapi.json
  - openapi/bond-pet-foods-store-openapi.json
  type: apiKey
- description: WordPress Application Password (username + generated password) sent as HTTP Basic.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/bond-pet-foods-content-openapi.json
  - openapi/bond-pet-foods-store-openapi.json
  type: http
slug: bond-pet-foods-authentication
source_filename: bond-pet-foods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: derived\nsource: openapi/bond-pet-foods-content-openapi.json, openapi/bond-pet-foods-store-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication nonce. Required for state-changing wp/v2 requests\n    from a logged-in browser session.\n  sources:\n  - openapi/bond-pet-foods-content-openapi.json\n  - openapi/bond-pet-foods-store-openapi.json\n- name: cartToken\n  type: apiKey\n  in: header\n  parameter: Cart-Token\n  description: WooCommerce Store API JWT session token identifying an anonymous cart. Returned\n    in the Cart-Token response header.\n  sources:\n  - openapi/bond-pet-foods-content-openapi.json\n  - openapi/bond-pet-foods-store-openapi.json\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Password (username + generated password)\
  \ sent as HTTP Basic.\n  sources:\n  - openapi/bond-pet-foods-content-openapi.json\n  - openapi/bond-pet-foods-store-openapi.json\ndocs:\n  status: not-published\n  detail: >-\n    Bond Pet Foods publishes no developer portal and no authentication documentation. The schemes\n    above are the WordPress/WooCommerce platform defaults, derived from the route index the host\n    itself serves and confirmed against live anonymous requests.\nobserved:\n  probed: '2026-08-08'\n  anonymous_read_allowed:\n  - GET /wp-json/wc/store/v1/products -> 200\n  - GET /wp-json/wc/store/v1/products/categories -> 200\n  - GET /wp-json/wc/store/v1/cart -> 200\n  - GET /wp-json/wp/v2/posts -> 200\n  - GET /wp-json/wp/v2/pages -> 200\n  - GET /wp-json/wp/v2/media -> 200\n  - GET /wp-json/wp/v2/search -> 200\n  credential_gated:\n  - GET /wp-json/wp/v2/users -> 401 rest_user_cannot_view\n  - GET /wp-json/wp/v2/settings -> 401 rest_forbidden\n  - GET /wp-json/wp-abilities/v1/abilities -> 401\n  - GET /wp-json/wp-abilities/v1/categories\
  \ -> 401\n  cors:\n    access_control_allow_origin: '*'\n    access_control_allow_credentials: true\n    allowed_headers: [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type, Cart-Token, Nonce]\n  oauth:\n    present: false\n    detail: >-\n      No OAuth or OpenID Connect surface exists. /.well-known/oauth-authorization-server,\n      /.well-known/oauth-protected-resource and /.well-known/openid-configuration all return 404,\n      and the discovery index advertises no OAuth namespace. No scopes/ artifact was written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/authentication/bond-pet-foods-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Pet Food
- Alternative Protein
- Precision Fermentation
- Food Technology
- Biotechnology
- Animal Nutrition
- Sustainability
- E-Commerce
- WooCommerce
- WordPress
---
