---
api_key_in: []
api_specs:
- filename: bioaegis-therapeutics-blocks-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Blocks API
  slug: bioaegis-therapeutics-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-blocks-api-openapi.yml
- filename: bioaegis-therapeutics-comments-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Comments API
  slug: bioaegis-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-comments-api-openapi.yml
- filename: bioaegis-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Discovery API
  slug: bioaegis-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-discovery-api-openapi.yml
- filename: bioaegis-therapeutics-media-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Media API
  slug: bioaegis-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-media-api-openapi.yml
- filename: bioaegis-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Oembed API
  slug: bioaegis-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-oembed-api-openapi.yml
- filename: bioaegis-therapeutics-pages-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Pages API
  slug: bioaegis-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-pages-api-openapi.yml
- filename: bioaegis-therapeutics-posts-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Posts API
  slug: bioaegis-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-posts-api-openapi.yml
- filename: bioaegis-therapeutics-search-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Search API
  slug: bioaegis-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-search-api-openapi.yml
- filename: bioaegis-therapeutics-seo-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Seo API
  slug: bioaegis-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-seo-api-openapi.yml
- filename: bioaegis-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Taxonomy API
  slug: bioaegis-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Bioaegis Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: BioAegis Therapeutics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BioAegis Therapeutics
provider_slug: bioaegis-therapeutics
scheme_count: 1
schemes:
- advertised_at: https://www.bioaegistherapeutics.com/wp-json/
  authorization_endpoint: https://www.bioaegistherapeutics.com/wp-admin/authorize-application.php
  id: application-passwords
  note: Advertised in the REST index, but the authorization endpoint is behind wp-admin. There is no self-service signup, no OAuth flow, no API key issuance and no developer account of any kind. Recorded because the provider advertises it, not because it is reachable.
  scheme: basic
  type: http
  usable_by_third_party: false
slug: bioaegis-therapeutics-authentication
source_filename: bioaegis-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://www.bioaegistherapeutics.com/wp-json/ plus the WordPress REST\n  route index, 2026-08-07. BioAegis Therapeutics publishes no authentication documentation of its\n  own.\napi: bioaegis-therapeutics-content-api\nsummary: >-\n  The BioAegis Therapeutics content API declares exactly one authentication provider, and it is not\n  usable by a third party. The REST index at /wp-json/ returns\n  `\"authentication\": {\"application-passwords\": {\"endpoints\": {\"authorization\":\n  \"https://www.bioaegistherapeutics.com/wp-admin/authorize-application.php\"}}}` — WordPress\n  application passwords, whose authorization endpoint requires an existing wp-admin login. The 23\n  read operations catalogued in this repo require no credentials at all. Everything else — writes,\n  users, settings, menus, themes, plugins, templates, revisions, the wp-abilities/v1 capability\n  registry, wp-site-health/v1, wp-block-editor/v1,\
  \ redirection/v1 and the administrative half of\n  yoast/v1 — is refused anonymously, and the only credential paths are a logged-in WordPress\n  session cookie plus an X-WP-Nonce, or an application password issued from wp-admin. Neither is\n  obtainable by a third party and neither is documented publicly, so no usable scheme is asserted\n  here.\nschemes:\n- id: application-passwords\n  type: http\n  scheme: basic\n  usable_by_third_party: false\n  advertised_at: https://www.bioaegistherapeutics.com/wp-json/\n  authorization_endpoint: https://www.bioaegistherapeutics.com/wp-admin/authorize-application.php\n  note: >-\n    Advertised in the REST index, but the authorization endpoint is behind wp-admin. There is no\n    self-service signup, no OAuth flow, no API key issuance and no developer account of any kind.\n    Recorded because the provider advertises it, not because it is reachable.\nobserved:\n- surface: read operations in openapi/bioaegis-therapeutics-content-openapi.yml\n  auth_required:\
  \ false\n  evidence: 'All 23 modelled operations returned HTTP 200 with no Authorization header on 2026-08-07.'\n- surface: /wp/v2/users, /wp/v2/users/me\n  auth_required: true\n  status: 403\n  code: null\n  evidence: >-\n    Blocked at the edge by the Sucuri CloudProxy WAF, which answers with an HTML interstitial\n    (cdn.sucuri.net stylesheets) rather than a WordPress JSON error. This is the only operation on\n    the surface whose failure response is not JSON — a client parsing every response as JSON will\n    throw here rather than read an error code.\n- surface: /wp/v2/settings\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n- surface: /wp/v2/menus, /wp/v2/menu-items, /wp/v2/menu-locations\n  auth_required: true\n  status: 401\n  code: rest_cannot_view\n- surface: /wp/v2/themes\n  auth_required: true\n  status: 401\n  code: rest_cannot_view_themes\n- surface: /wp/v2/plugins\n  auth_required: true\n  status: 401\n  code: rest_cannot_view_plugins\n- surface: /wp/v2/templates,\
  \ /wp/v2/template-parts\n  auth_required: true\n  status: 401\n  code: rest_cannot_manage_templates\n- surface: /wp/v2/global-styles/themes/astra\n  auth_required: true\n  status: 401\n  code: rest_cannot_read_global_styles\n- surface: /wp/v2/block-types\n  auth_required: true\n  status: 401\n  code: rest_block_type_cannot_view\n- surface: /wp/v2/block-patterns/categories\n  auth_required: true\n  status: 401\n  code: rest_cannot_view\n- surface: /wp/v2/pattern-directory/patterns\n  auth_required: true\n  status: 401\n  code: rest_pattern_directory_cannot_view\n- surface: /wp/v2/sidebars, /wp/v2/widget-types\n  auth_required: true\n  status: 401\n  code: rest_cannot_manage_widgets\n- surface: /wp/v2/font-collections\n  auth_required: true\n  status: 401\n  code: rest_cannot_read\n- surface: /wp/v2/posts/{id}/revisions\n  auth_required: true\n  status: 401\n  code: rest_cannot_read\n- surface: /oembed/1.0/proxy\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: The oEmbed\
  \ provider endpoint (/oembed/1.0/embed) is anonymous; only the third-party proxy is gated.\n- surface: /yoast/v1/available_posts\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: >-\n    52 of the 53 yoast/v1 routes are administrative. Only /yoast/v1/get_head answers anonymously.\n- surface: /wp-site-health/v1/*\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n- surface: /wp-block-editor/v1/export\n  auth_required: true\n  status: 401\n  code: rest_cannot_export_templates\n- surface: /redirection/v1/redirect\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n- surface: /wp-abilities/v1/abilities, /wp-abilities/v1/categories\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API — an agent-facing capability registry — is registered on this\n    deployment but every endpoint under it, including the read-only /abilities and /categories\n    listings, refuses anonymous callers. The namespace\
  \ index /wp-abilities/v1 itself returns 200\n    with route metadata only. No agent surface is claimed for this provider.\n- surface: /elementor/v1/globals\n  auth_required: unknown\n  status: 500\n  note: Returns a server error rather than an auth error anonymously.\n- surface: /astra/v1/get-sites\n  auth_required: unknown\n  status: 502\n  note: Returns a bad-gateway from the WAF/origin rather than an auth error anonymously.\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    HTTPS is enforced and TLS 1.3 negotiates, but no Strict-Transport-Security header is served on\n    the API host, so a first-contact downgrade is not prevented. See\n    security/bioaegis-therapeutics-domain-security.yml.\ndocs: null\ndocs_note: >-\n  BioAegis Therapeutics publishes no authentication documentation for this surface. The upstream\n  contract is defined by the WordPress REST handbook at\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/authentication/bioaegis-therapeutics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- biopharmaceuticals
- Biotechnology
- Clinical Trials
- Immunology
- inflammation
- Innate Immunity
- gelsolin
- Protein Therapeutics
- ards
- Critical Care
- Rare Disease
- Drug Development
- Life Sciences
- content-api
---
