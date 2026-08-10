---
api_key_in: []
api_specs:
- filename: alloplex-biotherapeutics-discovery-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Discovery API
  slug: alloplex-biotherapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-discovery-api-openapi.yml
- filename: alloplex-biotherapeutics-media-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Media API
  slug: alloplex-biotherapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-media-api-openapi.yml
- filename: alloplex-biotherapeutics-oembed-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Oembed API
  slug: alloplex-biotherapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-oembed-api-openapi.yml
- filename: alloplex-biotherapeutics-pages-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Pages API
  slug: alloplex-biotherapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-pages-api-openapi.yml
- filename: alloplex-biotherapeutics-posts-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Posts API
  slug: alloplex-biotherapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-posts-api-openapi.yml
- filename: alloplex-biotherapeutics-search-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Search API
  slug: alloplex-biotherapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-search-api-openapi.yml
- filename: alloplex-biotherapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Taxonomy API
  slug: alloplex-biotherapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Alloplex Biotherapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloplex Biotherapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Alloplex Biotherapeutics
provider_slug: alloplex-biotherapeutics
scheme_count: 0
schemes: []
slug: alloplex-biotherapeutics-authentication
source_filename: alloplex-biotherapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://alloplexbio.com/wp-json/ plus the WordPress REST route index,\n  2026-08-06. Alloplex Biotherapeutics publishes no authentication documentation of its own.\napi: alloplex-biotherapeutics-content-api\nsummary: >-\n  The Alloplex Biotherapeutics content API declares NO authentication schemes. The REST index at\n  /wp-json/ returns `\"authentication\": []`, meaning WordPress core has no application-password or\n  other REST authentication provider registered for anonymous negotiation. The read operations\n  catalogued in this repo require no credentials at all. Everything else — writes, users, settings,\n  menus, menu-items, templates, block-types, font-families, plugins, themes, widgets, sidebars,\n  revisions, autosaves, the `mcp` MCP-adapter namespace, the `wp-abilities/v1` capability registry,\n  `wordfence/v1`, `rankmath/v1`, `post-duplicator/v1`, `wpe_sign_on_plugin/v1`,\n  `wpe/cache-plugin/v1`,\
  \ `wp-site-health/v1` and `wp-block-editor/v1` — is refused anonymously with\n  a WordPress capability error. The only credential path is a logged-in WordPress session cookie\n  plus an X-WP-Nonce, or an application password issued from wp-admin. Neither is obtainable by a\n  third party, and neither is documented publicly, so no scheme is asserted here.\nschemes: []\nobserved:\n- surface: read operations in openapi/alloplex-biotherapeutics-content-openapi.yml\n  auth_required: false\n  evidence: 'All 19 modelled operations returned HTTP 200 with no Authorization header on 2026-08-06.'\n- surface: /wp/v2/users\n  auth_required: true\n  status: 401\n  code: rest_user_cannot_view\n  evidence: 'Sorry, you are not allowed to list users.'\n- surface: /wp/v2/settings\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  evidence: 'Sorry, you are not allowed to do that.'\n- surface: /wp/v2/menus, /wp/v2/menu-items\n  auth_required: true\n  status: 401\n- surface: /wp/v2/templates,\
  \ /wp/v2/block-types, /wp/v2/font-families, /wp/v2/plugins, /wp/v2/themes, /wp/v2/widgets, /wp/v2/sidebars, /wp/v2/pattern-directory/patterns\n  auth_required: true\n  status: 401\n- surface: /wp/v2/posts/{id}/revisions, /wp/v2/pages/{id}/revisions, autosaves\n  auth_required: true\n  status: 401\n- surface: /mcp/mcp-adapter-default-server\n  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The site installs the WordPress MCP adapter and registers a Streamable-HTTP MCP endpoint at\n    POST /wp-json/mcp/mcp-adapter-default-server. Both `initialize` and `tools/list` JSON-RPC calls\n    were refused anonymously with 401 rest_forbidden, so the live tool set and its inputSchemas\n    could not be introspected. NO MCP server artifact is claimed for this provider: the endpoint is\n    a WordPress plugin default, not a hosted MCP product Alloplex markets, and its tools are not\n    publicly enumerable.\n- surface: /wp-abilities/v1/abilities, /wp-abilities/v1/categories\n\
  \  auth_required: true\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API — an agent-facing capability registry — is registered on this\n    deployment but every endpoint under it, including the read-only /abilities and /categories\n    listings, refuses anonymous callers. No agent surface is claimed for this provider.\n- surface: /wordfence/v1/*, /rankmath/v1/*, /post-duplicator/v1/*, /wpe_sign_on_plugin/v1/*, /wpe/cache-plugin/v1/*, /wp-site-health/v1/*, /wp-block-editor/v1/*\n  auth_required: true\n  status: 401\n- surface: /batch/v1\n  auth_required: true\n  status: 403\n  note: The WordPress REST batch endpoint is registered but refuses anonymous callers.\n- surface: /wp/v2/comments\n  auth_required: false\n  status: 200\n  note: >-\n    Not an auth wall — the collection is readable and simply empty (X-WP-Total 0) because comments\n    are closed site-wide.\ncredential_issuance:\n  self_service: false\n  note: >-\n    There is no signup, no developer\
  \ portal, no API key issuance and no OAuth client registration.\n    Alloplex Biotherapeutics does not market this surface as an API; it is the WordPress content\n    surface its own site runs on. The site does operate a gated shareholder portal at\n    /portal-login/, but that is a human web login for investors, not an API credential path.\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  hsts: false\n  cdn: Cloudflare in front of WP Engine origin\n  note: >-\n    No Strict-Transport-Security header is sent, so HTTPS is not pinned for a first-time client.\n    Responses carry `x-content-type-options: nosniff` and an\n    `access-control-allow-headers: Authorization, X-WP-Nonce, ...` preflight allowance, which is the\n    standard WordPress cookie+nonce credential path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/authentication/alloplex-biotherapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- biotechnology
- cell-therapy
- immunotherapy
- oncology
- cancer
- clinical-trials
- life-sciences
- drug-development
- autoimmunity
- content-api
---
