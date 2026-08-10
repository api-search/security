---
api_key_in: []
api_specs:
- filename: jenavalve-technology-authors-api-openapi.yml
  format: yaml
  label: JenaValve Technology Authors API
  slug: jenavalve-technology-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-authors-api-openapi.yml
- filename: jenavalve-technology-content-api-openapi.yml
  format: yaml
  label: JenaValve Technology Content API
  slug: jenavalve-technology-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-content-api-openapi.yml
- filename: jenavalve-technology-discovery-api-openapi.yml
  format: yaml
  label: JenaValve Technology Discovery API
  slug: jenavalve-technology-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-discovery-api-openapi.yml
- filename: jenavalve-technology-media-api-openapi.yml
  format: yaml
  label: JenaValve Technology Media API
  slug: jenavalve-technology-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-media-api-openapi.yml
- filename: jenavalve-technology-oembed-api-openapi.yml
  format: yaml
  label: JenaValve Technology O Embed API
  slug: jenavalve-technology-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-oembed-api-openapi.yml
- filename: jenavalve-technology-seo-api-openapi.yml
  format: yaml
  label: JenaValve Technology SEO API
  slug: jenavalve-technology-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-seo-api-openapi.yml
- filename: jenavalve-technology-taxonomy-api-openapi.yml
  format: yaml
  label: JenaValve Technology Taxonomy API
  slug: jenavalve-technology-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/openapi/jenavalve-technology-taxonomy-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: probed
name: Jenavalve Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: JenaValve Technology secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JenaValve Technology
provider_slug: jenavalve-technology
scheme_count: 2
schemes:
- description: The default and only posture for third parties. All described content operations — posts, pages, media, categories, tags, users, comments, search, types, taxonomies, statuses, blocks, navigation, oEmbed and the Yoast head endpoint — return HTTP 200 with no Authorization header.
  name: anonymous
  sources:
  - openapi/jenavalve-technology-site-openapi.yml
  - openapi/jenavalve-technology-discover-ar-openapi.yml
  type: none
- audience: site-editors-only
  authorization_endpoint: https://jenavalve.com/wp-admin/authorize-application.php
  description: WordPress application passwords, advertised in the /wp-json discovery document on jenavalve.com with an authorization endpoint at /wp-admin/authorize-application.php. This is an internal CMS-author credential issued only to the site's own WordPress users; it is NOT a public API credential and no third party can obtain one. Recorded because the site advertises it, not because it is available.
  name: application-passwords
  scheme: basic
  sources:
  - https://jenavalve.com/wp-json
  third_party_obtainable: false
  type: http
slug: jenavalve-technology-authentication
source_filename: jenavalve-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: >-\n  Anonymous probing of https://jenavalve.com/wp-json and https://discover-ar.com/wp-json plus\n  the `authentication` block of the WordPress route-discovery document.\nsummary:\n  types: [none, http]\n  anonymous_read: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    JenaValve publishes no API authentication scheme because it publishes no API programme.\n    There is no key issuance, no client registration, no OAuth authorization server, no OIDC\n    discovery document and no developer account of any kind. Every operation described in this\n    repo's OpenAPI files is reachable with NO credential at all. The only authentication\n    mechanism either site advertises is WordPress application passwords, which is a CMS-author\n    mechanism for the site's own two editors — not a consumer-facing API credential, and not\n    obtainable by a third party.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n\
  \    The default and only posture for third parties. All described content operations —\n    posts, pages, media, categories, tags, users, comments, search, types, taxonomies,\n    statuses, blocks, navigation, oEmbed and the Yoast head endpoint — return HTTP 200 with no\n    Authorization header.\n  sources:\n  - openapi/jenavalve-technology-site-openapi.yml\n  - openapi/jenavalve-technology-discover-ar-openapi.yml\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, advertised in the /wp-json discovery document on\n    jenavalve.com with an authorization endpoint at /wp-admin/authorize-application.php. This\n    is an internal CMS-author credential issued only to the site's own WordPress users; it is\n    NOT a public API credential and no third party can obtain one. Recorded because the site\n    advertises it, not because it is available.\n  authorization_endpoint: https://jenavalve.com/wp-admin/authorize-application.php\n\
  \  audience: site-editors-only\n  third_party_obtainable: false\n  sources:\n  - https://jenavalve.com/wp-json\naccess_posture:\n  description: >-\n    Both sites split cleanly between wide-open content routes and correctly locked\n    administrative routes. Unlike some WordPress deployments hardened by a security plugin,\n    nothing here 401s the standard content collections — the anonymous reader gets the full\n    published corpus.\n  anonymous_200:\n  - wp/v2/posts\n  - wp/v2/pages\n  - wp/v2/media\n  - wp/v2/categories\n  - wp/v2/tags\n  - wp/v2/users\n  - wp/v2/comments\n  - wp/v2/search\n  - wp/v2/types\n  - wp/v2/taxonomies\n  - wp/v2/statuses\n  - wp/v2/blocks\n  - wp/v2/navigation\n  - wp/v2/events\n  - oembed/1.0/embed\n  - yoast/v1/get_head (discover-ar.com only)\n  denied:\n  - route: wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - route: wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - route: wp/v2/menu-items\n    status: 401\n\
  \    code: rest_cannot_view\n  - route: wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n  - route: wp-site-health/v1/tests/background-updates\n    status: 401\n    code: rest_forbidden\n  - route: cky/v1/settings\n    status: 401\n    code: cookieyes_rest_cannot_view\n  - route: contact-form-7/v1/contact-forms\n    status: 403\n    code: wpcf7_forbidden\nobservations:\n- id: no-hsts\n  note: >-\n    Neither jenavalve.com nor discover-ar.com sets Strict-Transport-Security, so a first request\n    over http:// is not protected against downgrade. See\n    security/jenavalve-technology-domain-security.yml.\n- id: author-enumeration\n  note: >-\n    wp/v2/users answers anonymously and returns the site's two published author bylines. This is\n    WordPress default behaviour and returns only public byline fields — name, slug, link and\n    avatar — with no email address or role. It is noted as a standard hardening consideration,\n    not as a data exposure; no personal data\
  \ is reproduced in this repo.\n- id: write-methods-untested\n  note: >-\n    Anonymous responses carry `Allow: GET`. No write method was ever attempted against either\n    host. The OpenAPI files therefore describe read operations only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/authentication/jenavalve-technology-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Structural Heart
- TAVR
- Aortic Regurgitation
- Aortic Stenosis
- Heart Valves
- Clinical Trials
- Patient Education
- Private Company
---
