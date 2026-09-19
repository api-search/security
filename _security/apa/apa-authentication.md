---
anonymous_access: true
api_key_in: []
api_specs:
- filename: apa-discovery-api-openapi.yml
  format: yaml
  label: APA Corporation
  slug: apa-corporation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-discovery-api-openapi.yml
- filename: apa-ticker-api-openapi.yml
  format: yaml
  label: APA Corporation Ticker API
  slug: apa-ticker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-ticker-api-openapi.yml
- filename: apa-newsroom-api-openapi.yml
  format: yaml
  label: APA Corporation Newsroom API
  slug: apa-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-newsroom-api-openapi.yml
- filename: apa-leadership-api-openapi.yml
  format: yaml
  label: APA Corporation Leadership API
  slug: apa-leadership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-leadership-api-openapi.yml
- filename: apa-pages-api-openapi.yml
  format: yaml
  label: APA Corporation Pages API
  slug: apa-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-pages-api-openapi.yml
- filename: apa-feed-items-api-openapi.yml
  format: yaml
  label: APA Corporation Feed Items API
  slug: apa-feed-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-feed-items-api-openapi.yml
- filename: apa-taxonomy-api-openapi.yml
  format: yaml
  label: APA Corporation Taxonomy API
  slug: apa-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-taxonomy-api-openapi.yml
- filename: apa-authors-api-openapi.yml
  format: yaml
  label: APA Corporation Authors API
  slug: apa-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-authors-api-openapi.yml
- filename: apa-search-api-openapi.yml
  format: yaml
  label: APA Corporation Search API
  slug: apa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-search-api-openapi.yml
- filename: apa-media-api-openapi.yml
  format: yaml
  label: APA Corporation Media API
  slug: apa-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-media-api-openapi.yml
- filename: apa-o-embed-api-openapi.yml
  format: yaml
  label: APA Corporation o Embed API
  slug: apa-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-o-embed-api-openapi.yml
auth_types: []
description: 'Authentication profile for the APA Corporation REST surface at https://apacorp.com/wp-json. The headline fact is that there is none to obtain: every operation profiled in this repository was called anonymously on 2026-09-14 and answered 200 with real data. APA publishes no developer program, no API keys, no sign-up, no OAuth. The only credential the surface knows about is the WordPress application password, which the site''s own root document advertises, and which is needed only for the write methods and the context=edit projection that are deliberately out of scope here.'
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Apa Authentication
name_suffix: Authentication
oauth_flows: []
overview: APA Corporation declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: APA Corporation
provider_slug: apa
scheme_count: 2
schemes:
- applies_to:
  - openapi/apa-ticker-api-openapi.yml
  - openapi/apa-newsroom-api-openapi.yml
  - openapi/apa-leadership-api-openapi.yml
  - openapi/apa-pages-api-openapi.yml
  - openapi/apa-media-hub-api-openapi.yml
  - openapi/apa-feed-items-api-openapi.yml
  - openapi/apa-taxonomy-api-openapi.yml
  - openapi/apa-authors-api-openapi.yml
  - openapi/apa-search-api-openapi.yml
  - openapi/apa-oembed-api-openapi.yml
  - openapi/apa-discovery-api-openapi.yml
  description: The default and only mode needed for the 28 operations documented in this repository. No Authorization header, no cookie, no nonce. The server sets Access-Control-Allow-Origin "*" and Access-Control-Allow-Methods "GET" on these routes, so a browser on any origin can call them directly.
  id: anonymous
  label: Anonymous public read
  type: none
  verified:
    date: '2026-09-14'
    evidence: GET https://apacorp.com/wp-json/apa-ticker/v1/quote returned 200 application/json with no credentials; GET /wp/v2/posts returned 200 with X-WP-Total 51; GET /wp/v2/leaderships returned 200 with X-WP-Total 25.
    method: live anonymous GET
- authorization_endpoint: https://apacorp.com/wp-admin/authorize-application.php
  description: HTTP Basic with a WordPress username and an application password. This is not an API-product credential — it is the WordPress account mechanism, issued from the site's own admin, and it exists for editors rather than for integrators. It unlocks the write methods and the context=edit field projection. No public route to obtain one exists for a third party.
  id: application-password
  label: WordPress application password
  obtainable_by_third_party: false
  required_for_documented_operations: false
  scheme: basic
  source: 'Declared verbatim by the provider at https://apacorp.com/wp-json/ under the top-level "authentication" key: {"application-passwords": {"endpoints": {"authorization": "https://apacorp.com/wp-admin/authorize-application.php"}}}'
  type: http
slug: apa-authentication
source_filename: apa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://apacorp.com/wp-json/ (the site's own root discovery document) + live anonymous calls to every documented operation\nprovider: APA Corporation\nproviderId: apa\ndescription: >-\n  Authentication profile for the APA Corporation REST surface at https://apacorp.com/wp-json. The\n  headline fact is that there is none to obtain: every operation profiled in this repository was\n  called anonymously on 2026-09-14 and answered 200 with real data. APA publishes no developer\n  program, no API keys, no sign-up, no OAuth. The only credential the surface knows about is the\n  WordPress application password, which the site's own root document advertises, and which is needed\n  only for the write methods and the context=edit projection that are deliberately out of scope here.\nsummary:\n  public_read: true\n  credential_required_for_documented_operations: false\n  signup_url: null\n  developer_program: false\n  schemes_declared: 1\n\
  schemes:\n  - id: anonymous\n    type: none\n    label: Anonymous public read\n    description: >-\n      The default and only mode needed for the 28 operations documented in this repository. No\n      Authorization header, no cookie, no nonce. The server sets Access-Control-Allow-Origin \"*\"\n      and Access-Control-Allow-Methods \"GET\" on these routes, so a browser on any origin can call\n      them directly.\n    applies_to:\n      - openapi/apa-ticker-api-openapi.yml\n      - openapi/apa-newsroom-api-openapi.yml\n      - openapi/apa-leadership-api-openapi.yml\n      - openapi/apa-pages-api-openapi.yml\n      - openapi/apa-media-hub-api-openapi.yml\n      - openapi/apa-feed-items-api-openapi.yml\n      - openapi/apa-taxonomy-api-openapi.yml\n      - openapi/apa-authors-api-openapi.yml\n      - openapi/apa-search-api-openapi.yml\n      - openapi/apa-oembed-api-openapi.yml\n      - openapi/apa-discovery-api-openapi.yml\n    verified:\n      method: live anonymous GET\n      date: '2026-09-14'\n\
  \      evidence: >-\n        GET https://apacorp.com/wp-json/apa-ticker/v1/quote returned 200 application/json with no\n        credentials; GET /wp/v2/posts returned 200 with X-WP-Total 51; GET /wp/v2/leaderships returned\n        200 with X-WP-Total 25.\n  - id: application-password\n    type: http\n    scheme: basic\n    label: WordPress application password\n    description: >-\n      HTTP Basic with a WordPress username and an application password. This is not an API-product\n      credential — it is the WordPress account mechanism, issued from the site's own admin, and it\n      exists for editors rather than for integrators. It unlocks the write methods and the\n      context=edit field projection. No public route to obtain one exists for a third party.\n    authorization_endpoint: https://apacorp.com/wp-admin/authorize-application.php\n    source: >-\n      Declared verbatim by the provider at https://apacorp.com/wp-json/ under the top-level\n      \"authentication\" key: {\"application-passwords\"\
  : {\"endpoints\": {\"authorization\":\n      \"https://apacorp.com/wp-admin/authorize-application.php\"}}}\n    required_for_documented_operations: false\n    obtainable_by_third_party: false\nnot_present:\n  - id: oauth2\n    note: No OAuth 2.0 surface. /.well-known/oauth-authorization-server returns 404 on apacorp.com and www.apacorp.com.\n  - id: oidc\n    note: No OpenID Connect surface. /.well-known/openid-configuration returns 404 on apacorp.com and www.apacorp.com.\n  - id: api-key\n    note: No API key issuance. There is no developer portal, no key management page and no sign-up.\n  - id: mtls\n    note: No mutual-TLS surface advertised or observed.\naccess_boundaries:\n  - boundary: context=edit\n    status: 401\n    code: rest_forbidden_context\n    note: Anonymous callers may request context=view or context=embed only.\n  - boundary: /wp/v2/menus\n    status: 401\n    code: rest_cannot_view\n    note: >-\n      Observed live on 2026-09-14 — \"Sorry, you are not allowed to view\
  \ menus.\" This route is\n      registered but not anonymously readable, and is deliberately excluded from the OpenAPIs here.\n  - boundary: write methods\n    status: 401\n    note: >-\n      POST, PUT, PATCH and DELETE exist on the wp/v2 routes but require an application password.\n      Nothing in this repository documents them; the public contract is read-only.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/authentication/apa-authentication.yml
summary_line: 2 schemes
tags:
- Oil and Gas
- Energy
- Exploration
- Production
- WordPress
- REST
- Content
- Newsroom
- Investor Relations
- Energy Production
---
