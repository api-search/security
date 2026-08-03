---
api_key_in:
- header
api_specs:
- filename: atsena-therapeutics-wp-rest-openapi.yml
  format: yaml
  label: Atsena Therapeutics Content API
  slug: atsena-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atsena-therapeutics/refs/heads/main/openapi/atsena-therapeutics-wp-rest-openapi.yml
auth_types:
- none
- http
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Atsena Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atsena Therapeutics secures its APIs with none, http, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Atsena Therapeutics
provider_slug: atsena-therapeutics
scheme_count: 3
schemes:
- description: 'The default and only scheme a third party can use. All 20 read operations in openapi/atsena-therapeutics-wp-rest-openapi.yml were verified to return HTTP 200 with no credentials on 2026-08-02 — posts, pages, media, categories, tags, search, the type/taxonomy/ status discovery endpoints, the route index and oEmbed. The spec carries a top-level `security: [{}]` to state this explicitly.'
  name: anonymous
  sources:
  - openapi/atsena-therapeutics-wp-rest-openapi.yml
  type: none
- description: WordPress application passwords — the only scheme the site advertises, published in the route index under authentication['application-passwords'] with an authorization endpoint at https://atsenatx.com/wp-admin/authorize-application.php. This is an administrative credential minted per WordPress user inside wp-admin; there is no self-service signup and no way for an external developer to obtain one. It guards the write operations and the privileged reads listed under `gated_surfaces` below.
  name: applicationPassword
  obtain: https://atsenatx.com/wp-admin/authorize-application.php
  scheme: basic
  self_service: false
  sources:
  - openapi/atsena-therapeutics-wp-rest-discovery-original.json
  type: http
- description: WordPress cookie-authentication nonce, used by the site's own logged-in admin UI rather than by API clients. Not advertised in the route index; observed in the live `Access-Control-Allow-Headers` response header on every wp-json response (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - live response headers on https://atsenatx.com/wp-json/wp/v2/posts
  type: apiKey
slug: atsena-therapeutics-authentication
source_filename: atsena-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: >-\n  openapi/atsena-therapeutics-wp-rest-openapi.yml, the live route-discovery document at\n  https://atsenatx.com/wp-json/, and live response headers observed 2026-08-02\nsummary:\n  types:\n    - none\n    - http\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  anonymous_read: true\n  headline: >-\n    Every operation modelled in this repo is anonymous. Atsena Therapeutics publishes no developer\n    program, issues no API keys and runs no OAuth authorization server; the only credentials this\n    surface understands are WordPress administrative ones, which are not available to third parties.\nschemes:\n  - name: anonymous\n    type: none\n    description: >-\n      The default and only scheme a third party can use. All 20 read operations in\n      openapi/atsena-therapeutics-wp-rest-openapi.yml were verified to return HTTP 200 with no\n      credentials on 2026-08-02 — posts, pages, media, categories, tags,\
  \ search, the type/taxonomy/\n      status discovery endpoints, the route index and oEmbed. The spec carries a top-level\n      `security: [{}]` to state this explicitly.\n    sources:\n      - openapi/atsena-therapeutics-wp-rest-openapi.yml\n  - name: applicationPassword\n    type: http\n    scheme: basic\n    description: >-\n      WordPress application passwords — the only scheme the site advertises, published in the route\n      index under authentication['application-passwords'] with an authorization endpoint at\n      https://atsenatx.com/wp-admin/authorize-application.php. This is an administrative credential\n      minted per WordPress user inside wp-admin; there is no self-service signup and no way for an\n      external developer to obtain one. It guards the write operations and the privileged reads\n      listed under `gated_surfaces` below.\n    obtain: https://atsenatx.com/wp-admin/authorize-application.php\n    self_service: false\n    sources:\n      - openapi/atsena-therapeutics-wp-rest-discovery-original.json\n\
  \  - name: wpNonce\n    type: apiKey\n    in: header\n    parameter: X-WP-Nonce\n    description: >-\n      WordPress cookie-authentication nonce, used by the site's own logged-in admin UI rather than by\n      API clients. Not advertised in the route index; observed in the live\n      `Access-Control-Allow-Headers` response header on every wp-json response\n      (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).\n    sources:\n      - live response headers on https://atsenatx.com/wp-json/wp/v2/posts\ngated_surfaces:\n  - path: /wp/v2/users\n    status: 401\n    code: rest_user_cannot_view\n    note: >-\n      Author identities are not disclosed anonymously, so the `author` id on a post or page cannot be\n      resolved without credentials.\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/plugins\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/templates\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menus\n\
  \    status: 401\n    code: rest_forbidden\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities registry — the agent-facing capability surface WordPress 6.8+ exposes —\n      is registered on this install but rejects anonymous callers. The namespace index at\n      /wp-abilities/v1 is readable (200); the abilities and categories collections beneath it are\n      not. No MCP namespace is registered on this install.\n  - path: /oembed/1.0/proxy\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/comments\n    status: 403\n    code: rest_comment_disabled\n    note: Comments are disabled site-wide, so the collection is unavailable to everyone, not just anonymous callers.\nabsent:\n  oauth2: >-\n    No OAuth. /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both\n    returned 404, and no scope surface exists anywhere on this host — scopes/ is deliberately not\n    emitted.\n  openid_connect:\
  \ '/.well-known/openid-configuration returned 404.'\n  api_keys: No API key programme, no key issuance, no developer account.\n  mtls: Not offered.\nx-evidence:\n  fetched: '2026-08-02'\n  anonymous_200_operations: 20\n  http_401_surfaces: 7\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atsena-therapeutics/refs/heads/main/authentication/atsena-therapeutics-authentication.yml
summary_line: none/http/apiKey · 3 schemes
tags:
- Company
- Biotechnology
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Ophthalmology
- Rare Disease
- Healthcare
- Research and Development
- Content API
- WordPress
---
