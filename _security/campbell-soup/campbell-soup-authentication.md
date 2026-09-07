---
anonymous_access: true
api_key_in: []
api_specs:
- filename: campbell-soup-content-api-openapi.yml
  format: yaml
  label: Campbell's Content API (WordPress REST)
  slug: campbells-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-content-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Campbell Soup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Campbell Soup declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Campbell Soup
provider_slug: campbell-soup
scheme_count: 2
schemes:
- applies_to: all GET operations
  evidence: 'GET https://www.campbells.com/wp-json/wp/v2/recipe?per_page=1 returned 200 with no Authorization header on 2026-09-05, carrying `Allow: GET` and `X-WP-Total: 316`.'
  id: anonymous
  type: none
- applies_to: all POST/PUT/PATCH/DELETE operations declared by the wp/v2 route document
  evidence: 'WordPress application passwords over HTTP Basic. The route discovery document declares the write methods and the surface exposes /wp/v2/users/{id}/application-passwords, but the live response advertises `Allow: GET` to anonymous callers and Campbell''s publishes no way for a third party to obtain credentials.'
  id: basicAuth
  public: false
  scheme: basic
  type: http
slug: campbell-soup-authentication
source_filename: campbell-soup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/campbell-soup-content-api-openapi.yml (derived from https://www.campbells.com/wp-json/wp/v2) + live anonymous probes\nprovider: The Campbell's Company\nproviderId: campbell-soup\nsummary: >-\n  The public surface is anonymous-read. Campbell's issues no developer credentials of any kind:\n  there is no signup, no key request, no OAuth server and no documented auth page. Reads require\n  nothing; writes are gated by WordPress core's own operator credentials, which are not available\n  to the public.\nschemes:\n  - id: anonymous\n    type: none\n    applies_to: all GET operations\n    evidence: >-\n      GET https://www.campbells.com/wp-json/wp/v2/recipe?per_page=1 returned 200 with no\n      Authorization header on 2026-09-05, carrying `Allow: GET` and `X-WP-Total: 316`.\n  - id: basicAuth\n    type: http\n    scheme: basic\n    applies_to: all POST/PUT/PATCH/DELETE operations declared by the wp/v2 route document\n   \
  \ public: false\n    evidence: >-\n      WordPress application passwords over HTTP Basic. The route discovery document declares the\n      write methods and the surface exposes /wp/v2/users/{id}/application-passwords, but the live\n      response advertises `Allow: GET` to anonymous callers and Campbell's publishes no way for a\n      third party to obtain credentials.\noauth: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nsignup_url: null\ndocs: null\nnotes: >-\n  The retired Campbell's Kitchen developer API (developer.campbellskitchen.com) issued API keys via\n  a developer portal. That host is NXDOMAIN as of 2026-09-05, so the key-issuing program is gone;\n  what survives is an unauthenticated read surface with no onboarding at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/authentication/campbell-soup-authentication.yml
summary_line: 2 schemes
tags:
- Food
- Consumer Packaged Goods
- Recipes
- Products
- Nutrition
- Brands
- Fortune 500
- Content API
- WordPress
---
