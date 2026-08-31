---
api_key_in: []
api_specs:
- filename: group14-technologies-discovery-api-openapi.yml
  format: yaml
  label: Group14 Technologies Discovery API
  slug: group14-technologies-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-discovery-api-openapi.yml
- filename: group14-technologies-job-openings-api-openapi.yml
  format: yaml
  label: Group14 Technologies Job Openings API
  slug: group14-technologies-job-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-job-openings-api-openapi.yml
- filename: group14-technologies-locations-api-openapi.yml
  format: yaml
  label: Group14 Technologies Locations API
  slug: group14-technologies-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-locations-api-openapi.yml
- filename: group14-technologies-media-api-openapi.yml
  format: yaml
  label: Group14 Technologies Media API
  slug: group14-technologies-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-media-api-openapi.yml
- filename: group14-technologies-pages-api-openapi.yml
  format: yaml
  label: Group14 Technologies Pages API
  slug: group14-technologies-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-pages-api-openapi.yml
- filename: group14-technologies-posts-api-openapi.yml
  format: yaml
  label: Group14 Technologies Posts API
  slug: group14-technologies-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-posts-api-openapi.yml
- filename: group14-technologies-resources-api-openapi.yml
  format: yaml
  label: Group14 Technologies Resources API
  slug: group14-technologies-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-resources-api-openapi.yml
- filename: group14-technologies-search-api-openapi.yml
  format: yaml
  label: Group14 Technologies Search API
  slug: group14-technologies-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-search-api-openapi.yml
- filename: group14-technologies-taxonomy-api-openapi.yml
  format: yaml
  label: Group14 Technologies Taxonomy API
  slug: group14-technologies-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-taxonomy-api-openapi.yml
- filename: group14-technologies-video-api-openapi.yml
  format: yaml
  label: Group14 Technologies Video API
  slug: group14-technologies-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-video-api-openapi.yml
auth_types: []
description: Group14 Technologies publishes no developer program, no API keys, no OAuth, no signup and no documentation of any kind for machine access. Everything below was read off live responses on 2026-08-22, not from a docs page, because there is no docs page.
kind: authentication
layout: security
method: probed
name: Group14 Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Group14 Technologies declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Group14 Technologies
provider_slug: group14-technologies
scheme_count: 3
schemes:
- applies_to: Every public read operation in openapi/ — resources, resource categories, pages, posts, categories, tags, job openings, job departments, job locations, locations, media, videos, video categories, search, types, taxonomies, statuses and the API index.
  detail: 'No key, token, header or account. Requests succeed unauthenticated and the collections answer `Allow: GET` without credentials.'
  evidence: 'GET https://group14.technology/wp-json/wp/v2/resource?per_page=1 -> 200, X-WP-Total: 169'
  name: anonymous
  type: none
- applies_to: The wp-admin surface and every write method on the same routes.
  detail: Logged-in WordPress session cookie plus an X-WP-Nonce header. `access-control-allow-headers` on every response advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`. There is no public path to a Group14 WordPress account.
  name: wordpress-cookie-nonce
  public_issuance: false
  type: cookie
- applies_to: Programmatic writes and the gated routes below.
  detail: WordPress application passwords over TLS (HTTP Basic). Issued only from the wp-admin profile screen of an existing account, so there is no third-party issuance path.
  name: wordpress-application-password
  public_issuance: false
  type: http-basic
slug: group14-technologies-authentication
source_filename: group14-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live responses from https://group14.technology/wp-json/ + the site's own REST index\ndescription: >-\n  Group14 Technologies publishes no developer program, no API keys, no OAuth, no signup and no\n  documentation of any kind for machine access. Everything below was read off live responses on\n  2026-08-22, not from a docs page, because there is no docs page.\nsummary:\n  public_read: true\n  credential_required_for_read: false\n  credential_issuance_path: none\n  registered_schemes: []\n  note: >-\n    The site's own REST index reports `\"authentication\": []` — WordPress core registers no\n    authentication scheme on this host beyond the built-in cookie and application-password paths.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: >-\n    Every public read operation in openapi/ — resources, resource categories, pages, posts,\n    categories, tags, job openings, job departments, job locations, locations, media, videos,\
  \ video\n    categories, search, types, taxonomies, statuses and the API index.\n  detail: >-\n    No key, token, header or account. Requests succeed unauthenticated and the collections answer\n    `Allow: GET` without credentials.\n  evidence: 'GET https://group14.technology/wp-json/wp/v2/resource?per_page=1 -> 200, X-WP-Total: 169'\n- name: wordpress-cookie-nonce\n  type: cookie\n  applies_to: The wp-admin surface and every write method on the same routes.\n  detail: >-\n    Logged-in WordPress session cookie plus an X-WP-Nonce header. `access-control-allow-headers` on\n    every response advertises `Authorization, X-WP-Nonce, Content-Disposition, Content-MD5,\n    Content-Type`. There is no public path to a Group14 WordPress account.\n  public_issuance: false\n- name: wordpress-application-password\n  type: http-basic\n  applies_to: Programmatic writes and the gated routes below.\n  detail: >-\n    WordPress application passwords over TLS (HTTP Basic). Issued only from the wp-admin\
  \ profile\n    screen of an existing account, so there is no third-party issuance path.\n  public_issuance: false\ngated_surfaces:\n- {path: /wp-json/wp/v2/users, status: 401, code: rest_forbidden, note: 'Author records are not exposed anonymously on this host — unusual, and a deliberate hardening.'}\n- {path: /wp-json/mcp/mcp-adapter-default-server, status: 401, code: rest_forbidden, note: 'The MCP Adapter endpoint. tools/list is unreadable without authentication.'}\n- {path: /wp-json/wp-abilities/v1/abilities, status: 401, code: rest_forbidden, note: The Abilities API backing the MCP adapter.}\n- {path: /wp-json/yoast/v1/*, status: 401, code: rest_forbidden, note: Yoast SEO plugin administration routes.}\n- {path: /wp-json/wordfence/v1/*, status: 401, code: rest_forbidden, note: 'Wordfence security plugin routes — present, gated.'}\noauth:\n  supported: false\n  discovery:\n  - {path: /.well-known/oauth-authorization-server, status: 404}\n  - {path: /.well-known/oauth-protected-resource,\
  \ status: 404}\n  - {path: /.well-known/openid-configuration, status: 404}\n  note: No OAuth or OIDC anywhere on this host. scopes/ is deliberately not written — there is no scope surface to record.\ntransport:\n  tls: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  note: See security/group14-technologies-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/authentication/group14-technologies-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Materials Science
- Battery Materials
- Silicon Anode
- Lithium-Ion
- Energy Storage
- Electric Vehicles
- Advanced Manufacturing
- Clean Energy
- Content
---
