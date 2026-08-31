---
api_key_in: []
api_specs:
- filename: adarx-pharmaceuticals-clinics-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Clinics API
  slug: adarx-pharmaceuticals-clinics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-clinics-api-openapi.yml
- filename: adarx-pharmaceuticals-content-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Content API
  slug: adarx-pharmaceuticals-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-content-api-openapi.yml
- filename: adarx-pharmaceuticals-embed-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Embed API
  slug: adarx-pharmaceuticals-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-embed-api-openapi.yml
- filename: adarx-pharmaceuticals-index-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Index API
  slug: adarx-pharmaceuticals-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-index-api-openapi.yml
- filename: adarx-pharmaceuticals-media-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Media API
  slug: adarx-pharmaceuticals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-media-api-openapi.yml
- filename: adarx-pharmaceuticals-people-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals People API
  slug: adarx-pharmaceuticals-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-people-api-openapi.yml
- filename: adarx-pharmaceuticals-search-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Search API
  slug: adarx-pharmaceuticals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-search-api-openapi.yml
- filename: adarx-pharmaceuticals-taxonomy-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Taxonomy API
  slug: adarx-pharmaceuticals-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-taxonomy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adarx Pharmaceuticals Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADARx Pharmaceuticals secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ADARx Pharmaceuticals
provider_slug: adarx-pharmaceuticals
scheme_count: 2
schemes:
- authorization_endpoints:
  - https://www.adarx.com/wp-admin/authorize-application.php
  - https://stophae.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords — HTTP Basic with a WordPress user login and a generated application password. Advertised by both route indexes under `authentication["application-passwords"].endpoints.authorization`, at https://www.adarx.com/wp-admin/authorize-application.php and https://stophae.com/wp-admin/authorize-application.php respectively. Required only for write and administrative routes, none of which are modelled in this repo. There is no public path to obtaining a credential — accounts are internal to ADARx.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/adarx-pharmaceuticals-content-openapi.yml
  - openapi/adarx-pharmaceuticals-stop-hae-openapi.yml
  type: http
- description: Cookie-plus-nonce authentication, used by the WordPress admin's own first-party JavaScript. Both hosts list X-WP-Nonce in `Access-Control-Allow-Headers`. Not usable by a third-party integrator — it requires a logged-in session cookie on the same origin.
  in: header
  name: wpNonce
  parameter_name: X-WP-Nonce
  sources:
  - live response headers, https://www.adarx.com/wp-json/wp/v2/posts
  type: apiKey
slug: adarx-pharmaceuticals-authentication
source_filename: adarx-pharmaceuticals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: >-\n  openapi/adarx-pharmaceuticals-content-openapi.yml,\n  openapi/adarx-pharmaceuticals-stop-hae-openapi.yml, and the `authentication` block returned by the\n  live route indexes at https://www.adarx.com/wp-json/ and https://stophae.com/wp-json/ on\n  2026-08-06.\nupstream_docs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nprovider_docs: null\nprovider_docs_note: >-\n  ADARx Pharmaceuticals publishes no authentication documentation of its own. The link above is the\n  upstream WordPress handbook that defines the scheme; it is recorded as `upstream_docs`, not as\n  `docs`, so it is never mistaken for a provider artifact.\nsummary:\n  types:\n  - http\n  public_read: true\n  api_key_in: []\n  oauth2_flows: []\n  oidc: false\n  mtls: false\npublic_access:\n  anonymous_read: true\n  detail: >-\n    Every operation catalogued in this repo — 24 on the content API and 17 on the STOP-HAE API —\n   \
  \ returns 200 without any credential. No API key, no token, no signup, no registration and no\n    rate-limit gate stands in front of them. There is nothing to obtain.\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords — HTTP Basic with a WordPress user login and a generated\n    application password. Advertised by both route indexes under\n    `authentication[\"application-passwords\"].endpoints.authorization`, at\n    https://www.adarx.com/wp-admin/authorize-application.php and\n    https://stophae.com/wp-admin/authorize-application.php respectively. Required only for write and\n    administrative routes, none of which are modelled in this repo. There is no public path to\n    obtaining a credential — accounts are internal to ADARx.\n  sources:\n  - openapi/adarx-pharmaceuticals-content-openapi.yml\n  - openapi/adarx-pharmaceuticals-stop-hae-openapi.yml\n  authorization_endpoints:\n  - https://www.adarx.com/wp-admin/authorize-application.php\n\
  \  - https://stophae.com/wp-admin/authorize-application.php\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description: >-\n    Cookie-plus-nonce authentication, used by the WordPress admin's own first-party JavaScript.\n    Both hosts list X-WP-Nonce in `Access-Control-Allow-Headers`. Not usable by a third-party\n    integrator — it requires a logged-in session cookie on the same origin.\n  sources:\n  - live response headers, https://www.adarx.com/wp-json/wp/v2/posts\nnot_present:\n- id: oauth2\n  evidence: /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource returned 404 on both hosts.\n- id: openIdConnect\n  evidence: /.well-known/openid-configuration returned 404 on both hosts.\n- id: apiKey-query\n  evidence: No query- or header-based API key is accepted or documented.\n- id: mutualTLS\n  evidence: No client-certificate requirement observed.\nauthorization_behaviour:\n  detail: >-\n    Refusals are capability-based and\
  \ arrive as HTTP 401 (not 403) with a WordPress error envelope —\n    `rest_forbidden`, `rest_cannot_read`, `rest_cannot_view_themes`, `rest_cannot_manage_widgets`\n    and siblings. Each object's `_links.self[].targetHints.allow` reports the methods available to\n    the current caller, which is `[\"GET\"]` anonymously. See\n    errors/adarx-pharmaceuticals-problem-types.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/authentication/adarx-pharmaceuticals-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- biotechnology
- biopharmaceuticals
- rna-therapeutics
- sirna
- rna-editing
- clinical-trials
- rare-disease
- drug-development
- life-sciences
- san-diego
- content-api
---
