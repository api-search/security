---
api_key_in: []
api_specs:
- filename: allotex-content-api-openapi.yml
  format: yaml
  label: Allotex Content API
  slug: allotex-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-content-api-openapi.yml
- filename: allotex-discovery-api-openapi.yml
  format: yaml
  label: Allotex Discovery API
  slug: allotex-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-discovery-api-openapi.yml
- filename: allotex-identity-api-openapi.yml
  format: yaml
  label: Allotex Identity API
  slug: allotex-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-identity-api-openapi.yml
- filename: allotex-media-api-openapi.yml
  format: yaml
  label: Allotex Media API
  slug: allotex-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-media-api-openapi.yml
- filename: allotex-schema-api-openapi.yml
  format: yaml
  label: Allotex Schema API
  slug: allotex-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-schema-api-openapi.yml
- filename: allotex-taxonomy-api-openapi.yml
  format: yaml
  label: Allotex Taxonomy API
  slug: allotex-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-taxonomy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Allotex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allotex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Allotex
provider_slug: allotex
scheme_count: 1
schemes:
- advertised_at: https://us.allotex.com/wp-json/
  authorization_endpoint: https://us.allotex.com/wp-admin/authorize-application.php
  description: WordPress application passwords over HTTP Basic - the only method the route index's `authentication` block advertises on either host. Credentials are minted from within the site's own wp-admin against an existing WordPress user account. Allotex operates no public signup, no developer registration and no key request form, so a third party has no route to a credential.
  name: applicationPassword
  required_by_any_catalogued_operation: false
  scheme: basic
  sources:
  - openapi/allotex-content-openapi.yml
  type: http
slug: allotex-authentication
source_filename: allotex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/allotex-content-openapi.yml\ncorroborated_by: https://us.allotex.com/wp-json/ (route index `authentication` block, fetched 2026-08-06)\napi: allotex:allotex-content-api\n\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\n  third_party_credential_obtainable: false\n\nheadline: >-\n  There is no developer authentication for Allotex. Every catalogued operation is readable\n  anonymously, and the one scheme the site advertises cannot be obtained by anyone outside the\n  company. This is not a gate you can get through - it is the absence of a developer program.\n\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  sources:\n  - openapi/allotex-content-openapi.yml\n  advertised_at: https://us.allotex.com/wp-json/\n  authorization_endpoint: https://us.allotex.com/wp-admin/authorize-application.php\n  description: >-\n    WordPress application\
  \ passwords over HTTP Basic - the only method the route index's\n    `authentication` block advertises on either host. Credentials are minted from within the site's\n    own wp-admin against an existing WordPress user account. Allotex operates no public signup, no\n    developer registration and no key request form, so a third party has no route to a credential.\n  required_by_any_catalogued_operation: false\n\nanonymous_surface:\n  detail: >-\n    All 25 operations in openapi/allotex-content-openapi.yml return 200 without any credential.\n  routes:\n  - /wp/v2/pages\n  - /wp/v2/posts\n  - /wp/v2/media\n  - /wp/v2/categories\n  - /wp/v2/tags\n  - /wp/v2/users\n  - /wp/v2/comments\n  - /wp/v2/search\n  - /wp/v2/types\n  - /wp/v2/taxonomies\n  - /wp/v2/statuses\n  - /wp/v2/blocks\n  - /wp/v2/navigation\n  - /oembed/1.0/embed\n  - /mcp\n\ngated_surface:\n  detail: >-\n    Probed anonymously on 2026-08-06. These are NOT retry-with-credentials conditions for a third\n    party - they are permanent.\n\
  \  routes:\n  - {path: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/menu-items, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/themes, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/plugins, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/block-patterns/patterns, status: 401, code: rest_forbidden}\n  - {path: /wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\n  - {path: /mcp/mcp-adapter-default-server, status: 401, code: rest_forbidden, method: POST}\n  - {path: /contact-form-7/v1/contact-forms, status: 403, code: wpcf7_forbidden}\n  - {path: '/wp/v2/pages?context=edit', status: 401, code: rest_forbidden_context}\n  - {path: /wp/v2/pages, status: 401, code: rest_cannot_create, method: POST}\n\nnot_supported:\n  oauth2:\n    supported: false\n    evidence: >-\n      No oauth2 securityScheme in the derived spec; /.well-known/oauth-authorization-server and\n      /.well-known/oauth-protected-resource both return 404 on both hosts.\n\
  \  openid_connect:\n    supported: false\n    evidence: /.well-known/openid-configuration returns 404 on both hosts.\n  api_keys:\n    supported: false\n    evidence: No apiKey scheme is advertised and no key issuance surface exists.\n  mutual_tls:\n    supported: false\n\ncsrf:\n  nonce_header: X-WP-Nonce\n  detail: >-\n    The route index's CORS policy allows an X-WP-Nonce request header, which is WordPress's\n    cookie-authenticated first-party mechanism for logged-in admin sessions. It is irrelevant to\n    third-party consumers, who have no session to nonce.\n\ndocs: null\ndocs_note: >-\n  Allotex publishes no authentication documentation. The upstream contract is defined at\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/ - that is WordPress's\n  documentation, not Allotex's, and is recorded as the humanURL on the API entry rather than as a\n  provider Documentation pointer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/authentication/allotex-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- medical-devices
- ophthalmology
- biologics
- vision-correction
- corneal-allograft
- presbyopia
- hyperopia
- refractive-surgery
- tissue-processing
- life-sciences
- clinical-trials
- content-api
---
