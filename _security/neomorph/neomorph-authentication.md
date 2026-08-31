---
api_key_in: []
api_specs:
- filename: neomorph-pages-api-openapi.yml
  format: yaml
  label: Neomorph Pages API
  slug: neomorph-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-pages-api-openapi.yml
- filename: neomorph-publications-api-openapi.yml
  format: yaml
  label: Neomorph Publications API
  slug: neomorph-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-publications-api-openapi.yml
- filename: neomorph-team-api-openapi.yml
  format: yaml
  label: Neomorph Team API
  slug: neomorph-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-team-api-openapi.yml
- filename: neomorph-media-api-openapi.yml
  format: yaml
  label: Neomorph Media API
  slug: neomorph-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-media-api-openapi.yml
- filename: neomorph-comments-api-openapi.yml
  format: yaml
  label: Neomorph Comments API
  slug: neomorph-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-comments-api-openapi.yml
- filename: neomorph-search-api-openapi.yml
  format: yaml
  label: Neomorph Search API
  slug: neomorph-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-search-api-openapi.yml
- filename: neomorph-discovery-api-openapi.yml
  format: yaml
  label: Neomorph Discovery API
  slug: neomorph-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-discovery-api-openapi.yml
- filename: neomorph-oembed-api-openapi.yml
  format: yaml
  label: Neomorph oEmbed API
  slug: neomorph-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-oembed-api-openapi.yml
- filename: neomorph-categories-api-openapi.yml
  format: yaml
  label: Neomorph Categories API
  slug: neomorph-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-categories-api-openapi.yml
- filename: neomorph-posts-api-openapi.yml
  format: yaml
  label: Neomorph Posts API
  slug: neomorph-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-posts-api-openapi.yml
- filename: neomorph-tags-api-openapi.yml
  format: yaml
  label: Neomorph Tags API
  slug: neomorph-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-tags-api-openapi.yml
- filename: neomorph-team-categories-api-openapi.yml
  format: yaml
  label: Neomorph Team Categories API
  slug: neomorph-team-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/openapi/neomorph-team-categories-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Neomorph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neomorph declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Neomorph
provider_slug: neomorph
scheme_count: 0
schemes: []
slug: neomorph-authentication
source_filename: neomorph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://neomorph.com/wp-json (route index + per-route OPTIONS\n  descriptors) on 2026-08-26, cross-read against the ten OpenAPI documents in openapi/.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  Every operation catalogued in this repo is anonymously readable and declares no security scheme.\n  Neomorph publishes no developer authentication documentation because it runs no developer program;\n  the read surface is simply open. The deployment's own REST index DOES advertise one authentication\n  provider for discovery — WordPress application passwords, with an authorization endpoint at\n  https://neomorph.com/wp-admin/authorize-application.php — but that is the CMS admin credential flow\n  for the site's own editors, not a developer-facing credential Neomorph issues to third parties. It\n  is recorded below because it is what the deployment says about\
  \ itself, not because it is an offered\n  API program. Application passwords are carried over HTTP Basic; the deployment also advertises\n  X-WP-Nonce in Access-Control-Allow-Headers for cookie-authenticated same-origin browser calls.\nschemes: []\nsite_declared_authentication:\n  provider: wordpress-application-passwords\n  transport: HTTP Basic (username + application password)\n  authorization_endpoint: https://neomorph.com/wp-admin/authorize-application.php\n  source_field: authentication (root of https://neomorph.com/wp-json/)\n  audience: site administrators and editors, not third-party developers\n  note: >-\n    Not exercised. The pipeline reads anonymously only and holds no credential for this deployment.\n  additional_credential_headers_advertised:\n  - Authorization\n  - X-WP-Nonce\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2/posts\n  - GET /wp/v2/posts/{id}\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET\
  \ /wp/v2/categories\n  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/comments\n  - GET /wp/v2/resource\n  - GET /wp/v2/resource/{id}\n  - GET /wp/v2/team\n  - GET /wp/v2/team/{id}\n  - GET /wp/v2/team_category\n  - GET /wp/v2/team_category/{id}\n  - GET /wp/v2/blocks\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/statuses\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/users\n    status: 403\n    code: null\n    note: >-\n      Blocked at the edge, not by the REST layer — the response is an HTML \"Forbidden Access\" page\n      from the site's WAF (WP Defender), not a JSON WP_Error envelope. This is the only gated route\n      on the deployment that does not answer in JSON.\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/menu-items\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/elementor_library\n\
  \    status: 401\n    code: rest_forbidden\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities API is registered on this deployment. It is the agent-facing capability\n      registry WordPress ships for MCP-style tool exposure, and it is entirely auth-gated here — no\n      ability names, descriptions or input schemas are readable anonymously.\n  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 432-route index requires an authenticated WordPress user.\n    None were exercised — the pipeline reads only.\nx-evidence:\n  probed: '2026-08-26'\n  index: https://neomorph.com/wp-json/\n  index_size_bytes: 649729\n  routes: 432\n  namespaces: 23\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://neomorph.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neomorph/refs/heads/main/authentication/neomorph-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Targeted Protein Degradation
- Molecular Glue
- Oncology
- Immunology
- Rare Disease
- Clinical Trials
- Life Sciences
- content-api
---
