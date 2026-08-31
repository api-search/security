---
api_key_in: []
api_specs:
- filename: nacuity-pharmaceuticals-discovery-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Discovery API
  slug: nacuity-pharmaceuticals-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-discovery-api-openapi.yml
- filename: nacuity-pharmaceuticals-media-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Media API
  slug: nacuity-pharmaceuticals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-media-api-openapi.yml
- filename: nacuity-pharmaceuticals-oembed-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Oembed API
  slug: nacuity-pharmaceuticals-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-oembed-api-openapi.yml
- filename: nacuity-pharmaceuticals-pages-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Pages API
  slug: nacuity-pharmaceuticals-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-pages-api-openapi.yml
- filename: nacuity-pharmaceuticals-portfolio-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Portfolio API
  slug: nacuity-pharmaceuticals-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-portfolio-api-openapi.yml
- filename: nacuity-pharmaceuticals-posts-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Posts API
  slug: nacuity-pharmaceuticals-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-posts-api-openapi.yml
- filename: nacuity-pharmaceuticals-search-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Search API
  slug: nacuity-pharmaceuticals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-search-api-openapi.yml
- filename: nacuity-pharmaceuticals-seo-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Seo API
  slug: nacuity-pharmaceuticals-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-seo-api-openapi.yml
- filename: nacuity-pharmaceuticals-taxonomy-api-openapi.yml
  format: yaml
  label: Nacuity Pharmaceuticals Taxonomy API
  slug: nacuity-pharmaceuticals-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/openapi/nacuity-pharmaceuticals-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Nacuity Pharmaceuticals Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nacuity Pharmaceuticals declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Nacuity Pharmaceuticals
provider_slug: nacuity-pharmaceuticals
scheme_count: 0
schemes: []
slug: nacuity-pharmaceuticals-authentication
source_filename: nacuity-pharmaceuticals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://www.nacuity.com/wp-json/ plus the WordPress REST route index,\n  2026-08-04. Nacuity Pharmaceuticals publishes no authentication documentation of its own.\napi: nacuity-pharmaceuticals-content-api\nsummary: >-\n  The Nacuity Pharmaceuticals content API declares NO authentication schemes. The REST index at\n  /wp-json/ returns `\"authentication\": []`, meaning WordPress core has no application-password or\n  other REST authentication provider registered for anonymous negotiation. The read operations\n  catalogued in this repo require no credentials at all. Everything else — writes, users, settings,\n  menus, themes, plugins, templates, the wp-abilities/v1 capability registry, wordfence/v1 and the\n  administrative half of yoast/v1 and exactmetrics/v1 — is refused anonymously with a WordPress\n  capability error, and the only credential path is a logged-in WordPress session cookie plus a\n\
  \  nonce, or an application password issued from wp-admin. Neither is obtainable by a third party,\n  and neither is documented publicly, so no scheme is asserted here.\nschemes: []\nobserved:\n- surface: read operations in openapi/nacuity-pharmaceuticals-content-openapi.yml\n  auth_required: false\n  evidence: 'All 22 modelled operations returned HTTP 200 with no Authorization header on 2026-08-04.'\n- surface: /wp/v2/users\n  auth_required: true\n  status: 401\n  code: rest_user_cannot_view\n  evidence: 'Sorry, you are not allowed to list users.'\n- surface: /wp/v2/settings\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n- surface: /wp/v2/menus, /wp/v2/menu-items, /wp/v2/menu-locations\n  auth_required: true\n  status: 401\n  code: rest_cannot_view\n- surface: /wp/v2/themes, /wp/v2/plugins, /wp/v2/templates, /wp/v2/block-types, /wp/v2/widgets, /wp/v2/widget-types, /wp/v2/sidebars, /wp/v2/icons, /wp/v2/font-collections, /wp/v2/block-patterns/patterns, /wp/v2/pattern-directory/patterns\n\
  \  auth_required: true\n  status: 401\n- surface: /wp-abilities/v1/*\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API — an agent-facing capability registry — is registered on this\n    deployment but every endpoint under it, including the read-only /abilities and /categories\n    listings, refuses anonymous callers. No agent surface is claimed for this provider.\n- surface: /wordfence/v1/*\n  auth_required: true\n  status: 401\n  code: rest_forbidden_context\n  evidence: 'Authorization header format is invalid.'\n- surface: /wp-site-health/v1/*\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n- surface: /wp/v2/comments\n  auth_required: false\n  status: 403\n  code: rest_comment_disabled\n  note: Not an auth wall — comments are switched off site-wide, so the collection is unavailable to anyone.\ncredential_issuance:\n  self_service: false\n  note: >-\n    There is no signup, no developer portal, no API key issuance\
  \ and no OAuth client registration.\n    Nacuity Pharmaceuticals does not market this surface as an API; it is the WordPress content\n    surface its own site runs on.\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.2\n  hsts: false\n  note: >-\n    The origin sends `Content-Security-Policy: upgrade-insecure-requests` but no\n    Strict-Transport-Security header, so HTTPS is not pinned for a first-time client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacuity-pharmaceuticals/refs/heads/main/authentication/nacuity-pharmaceuticals-authentication.yml
summary_line: 0 schemes
tags:
- Company
- biopharmaceuticals
- pharmaceuticals
- ophthalmology
- rare-disease
- clinical-trials
- retinitis-pigmentosa
- oxidative-stress
- life-sciences
- drug-development
- content-api
---
