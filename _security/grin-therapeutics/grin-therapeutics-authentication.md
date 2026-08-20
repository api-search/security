---
api_key_in: []
api_specs:
- filename: grin-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Discovery API
  slug: grin-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-discovery-api-openapi.yml
- filename: grin-therapeutics-media-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Media API
  slug: grin-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-media-api-openapi.yml
- filename: grin-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Oembed API
  slug: grin-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-oembed-api-openapi.yml
- filename: grin-therapeutics-pages-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Pages API
  slug: grin-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-pages-api-openapi.yml
- filename: grin-therapeutics-posts-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Posts API
  slug: grin-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-posts-api-openapi.yml
- filename: grin-therapeutics-search-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Search API
  slug: grin-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-search-api-openapi.yml
- filename: grin-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Taxonomy API
  slug: grin-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-taxonomy-api-openapi.yml
- filename: grin-therapeutics-users-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Users API
  slug: grin-therapeutics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-users-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Grin Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: GRIN Therapeutics secures its APIs with none and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GRIN Therapeutics
provider_slug: grin-therapeutics
scheme_count: 3
schemes:
- applies_to:
  - getApiIndex
  - listPosts
  - getPost
  - listPages
  - getPage
  - listMedia
  - getMediaItem
  - listCategories
  - getCategory
  - listTags
  - getTag
  - listUsers
  - getUser
  - searchContent
  - listTypes
  - getType
  - listTaxonomies
  - listStatuses
  - getOembed
  description: Every operation modelled in openapi/grin-therapeutics-content-openapi.yml was verified to return data with no Authorization header, no cookie and no nonce. Read access is unrestricted and unmetered as observed.
  name: anonymous
  sources:
  - openapi/grin-therapeutics-content-openapi.yml
  type: none
- authorization_endpoint: https://grintherapeutics.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords (HTTP Basic with a per-application credential). Advertised verbatim by the site's own REST index at https://grintherapeutics.com/wp-json/ as authentication.application-passwords.endpoints.authorization = https://grintherapeutics.com/wp-admin/authorize-application.php. This gates the write surface and the privileged read surface; it is an internal editorial credential, not a developer credential — GRIN Therapeutics offers no way for a third party to obtain one.
  name: application-passwords
  scheme: basic
  sources:
  - https://grintherapeutics.com/wp-json/
  type: http
- description: WordPress core's first-party session scheme for same-origin browser requests. Inferred from the Access-Control-Allow-Headers response header observed on the collection endpoints, which lists 'Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'. Not usable by a third-party integrator.
  in: header
  name: cookie-plus-nonce
  parameter_name: X-WP-Nonce
  sources:
  - https://grintherapeutics.com/wp-json/wp/v2/pages
  type: apiKey
slug: grin-therapeutics-authentication
source_filename: grin-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://grintherapeutics.com/wp-json/ (REST API index `authentication` block) plus live anonymous requests\nnote: >-\n  The OpenAPI in this repo declares no securitySchemes because the operations it models are the ones\n  that genuinely return data with no credentials — the read side of the WordPress REST content API is\n  fully anonymous. This profile records that anonymous-read model and the authenticated surface that\n  sits behind it, which the site's own REST index advertises. GRIN Therapeutics publishes no\n  developer authentication documentation of its own; the scheme below is WordPress core behaviour.\nsummary:\n  types: [none, http]\n  anonymous_read: true\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    Every operation modelled in openapi/grin-therapeutics-content-openapi.yml was verified to return\n    data with no Authorization\
  \ header, no cookie and no nonce. Read access is unrestricted and\n    unmetered as observed.\n  applies_to:\n  - getApiIndex\n  - listPosts\n  - getPost\n  - listPages\n  - getPage\n  - listMedia\n  - getMediaItem\n  - listCategories\n  - getCategory\n  - listTags\n  - getTag\n  - listUsers\n  - getUser\n  - searchContent\n  - listTypes\n  - getType\n  - listTaxonomies\n  - listStatuses\n  - getOembed\n  sources: [openapi/grin-therapeutics-content-openapi.yml]\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords (HTTP Basic with a per-application credential). Advertised\n    verbatim by the site's own REST index at https://grintherapeutics.com/wp-json/ as\n    authentication.application-passwords.endpoints.authorization =\n    https://grintherapeutics.com/wp-admin/authorize-application.php. This gates the write surface and\n    the privileged read surface; it is an internal editorial credential, not a developer credential\
  \ —\n    GRIN Therapeutics offers no way for a third party to obtain one.\n  authorization_endpoint: https://grintherapeutics.com/wp-admin/authorize-application.php\n  sources: [https://grintherapeutics.com/wp-json/]\n- name: cookie-plus-nonce\n  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description: >-\n    WordPress core's first-party session scheme for same-origin browser requests. Inferred from the\n    Access-Control-Allow-Headers response header observed on the collection endpoints, which lists\n    'Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'. Not usable by a\n    third-party integrator.\n  sources: [https://grintherapeutics.com/wp-json/wp/v2/pages]\ngated_surfaces:\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/users/me\n  status: 401\n  note: Requires an authenticated principal.\n- path: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API\
  \ — an agent-facing capability registry with a /run execution\n    endpoint — is registered on this site but is entirely credential-gated. No agent capability is\n    exposed to anonymous callers, so no MCP or agent-surface claim is made for this provider.\n- path: /wp-abilities/v1/categories\n  status: 401\n  code: rest_forbidden\n- path: /contact-form-7/v1/contact-forms\n  status: 403\n  code: wpcf7_forbidden\n- path: /wp/v2/comments\n  status: 403\n  code: rest_comment_disabled\n  note: Comments are disabled site-wide, so the comments collection is unreadable rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/authentication/grin-therapeutics-authentication.yml
summary_line: none/http · 3 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Neuroscience
- Rare Disease
- Precision Medicine
- Clinical Trials
- Pediatrics
- Epilepsy
- Life Sciences
- content-api
---
