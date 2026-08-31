---
api_key_in: []
api_specs:
- filename: leaf4life-pages-api-openapi.yml
  format: yaml
  label: LEAF4Life Content Pages API
  slug: leaf4life-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-pages-api-openapi.yml
- filename: leaf4life-media-api-openapi.yml
  format: yaml
  label: LEAF4Life Media API
  slug: leaf4life-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-media-api-openapi.yml
- filename: leaf4life-taxonomy-api-openapi.yml
  format: yaml
  label: LEAF4Life Taxonomy API
  slug: leaf4life-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-taxonomy-api-openapi.yml
- filename: leaf4life-discovery-api-openapi.yml
  format: yaml
  label: LEAF4Life API Discovery
  slug: leaf4life-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-discovery-api-openapi.yml
- filename: leaf4life-search-api-openapi.yml
  format: yaml
  label: LEAF4Life Search API
  slug: leaf4life-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-search-api-openapi.yml
- filename: leaf4life-users-api-openapi.yml
  format: yaml
  label: LEAF4Life Authors API
  slug: leaf4life-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-users-api-openapi.yml
- filename: leaf4life-posts-api-openapi.yml
  format: yaml
  label: LEAF4Life Posts and Comments API
  slug: leaf4life-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-posts-api-openapi.yml
- filename: leaf4life-oembed-api-openapi.yml
  format: yaml
  label: LEAF4Life oEmbed API
  slug: leaf4life-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-oembed-api-openapi.yml
- filename: leaf4life-comments-api-openapi.yml
  format: yaml
  label: LEAF4Life Comments API
  slug: leaf4life-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-comments-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Leaf4Life Authentication
name_suffix: Authentication
oauth_flows: []
overview: LEAF4Life declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LEAF4Life
provider_slug: leaf4life
scheme_count: 1
schemes:
- authorization_endpoint: https://leafforlife.com/wp-admin/authorize-application.php
  detail: Declared verbatim by the route index as authentication.application-passwords.endpoints.authorization. WordPress application passwords are per-user credentials issued from the site's own admin screen to an already-authenticated editor. There is no self-service registration, no client-credentials grant, no key issuance and no developer signup, so this cannot be treated as a public API authentication scheme. It is recorded because it is what the provider actually publishes.
  header: Authorization
  id: applicationPassword
  in: header
  obtainable_by_third_party: false
  provider_advertised: true
  scheme: basic
  type: http
slug: leaf4life-authentication
source_filename: leaf4life-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: >-\n  Live WordPress REST route index at https://leafforlife.com/wp-json/ plus anonymous probes of every\n  namespace on 2026-08-25, cross-checked against the OpenAPI documents in openapi/.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nnote: >-\n  The LEAF4Life content API declares no security schemes and requires no credentials for any operation\n  catalogued in this repo. LEAF4Life runs no developer program and publishes no authentication\n  documentation, because there is no product API to authenticate against — the read surface is simply\n  open. The one authentication mechanism the deployment advertises for discovery is WordPress\n  application passwords (HTTP Basic over TLS), announced in the `authentication` block of the route\n  index and pointing at the wp-admin authorization screen. That mechanism exists for the site's own\n  editors; it is not an API credential a third party can\
  \ obtain, and no attempt was made to use it.\nschemes:\n- id: applicationPassword\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  provider_advertised: true\n  obtainable_by_third_party: false\n  authorization_endpoint: https://leafforlife.com/wp-admin/authorize-application.php\n  detail: >-\n    Declared verbatim by the route index as\n    authentication.application-passwords.endpoints.authorization. WordPress application passwords are\n    per-user credentials issued from the site's own admin screen to an already-authenticated editor.\n    There is no self-service registration, no client-credentials grant, no key issuance and no\n    developer signup, so this cannot be treated as a public API authentication scheme. It is recorded\n    because it is what the provider actually publishes.\nanonymous_access:\n  readable:\n  - GET /\n  - GET /wp/v2\n  - GET /wp/v2/pages\n  - GET /wp/v2/pages/{id}\n  - GET /wp/v2/media\n  - GET /wp/v2/media/{id}\n  - GET /wp/v2/categories\n\
  \  - GET /wp/v2/categories/{id}\n  - GET /wp/v2/tags\n  - GET /wp/v2/tags/{id}\n  - GET /wp/v2/posts\n  - GET /wp/v2/comments\n  - GET /wp/v2/blocks\n  - GET /wp/v2/navigation\n  - GET /wp/v2/search\n  - GET /wp/v2/types\n  - GET /wp/v2/taxonomies\n  - GET /wp/v2/statuses\n  - GET /wp/v2/users\n  - GET /oembed/1.0/embed\n  gated:\n  - path: /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp/v2/menu-items\n    status: 401\n    code: rest_cannot_view\n  - path: /wp/v2/template-parts\n    status: 401\n    code: rest_cannot_manage_templates\n  - path: /wp/v2/pages?context=edit\n    status: 401\n    code: rest_forbidden_context\n    note: The `edit` context is closed anonymously; `view` and `embed` return data.\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    note: >-\n      The WordPress Abilities API namespace is registered on this deployment (WordPress\
  \ 7.0.3) but\n      closed to anonymous callers. It is the nearest thing to an agent-callable tool registry here,\n      and it is not reachable without credentials, so no tool schemas could be read.\n  - path: /wp-abilities/v1/categories\n    status: 401\n    code: rest_forbidden\n  - path: /wp-site-health/v1/tests/background-updates\n    status: 401\n    code: rest_forbidden\n  - path: /akismet/v1/key\n    status: 401\n    code: rest_forbidden\n  - path: /wp-super-cache/v1/settings\n    status: 401\n    code: rest_forbidden\n  write_operations: >-\n    Every POST/PUT/PATCH/DELETE route in the 150-route index requires an authenticated WordPress user.\n    None were exercised — this pipeline reads only.\nx-evidence:\n  probed: '2026-08-25'\n  index: https://leafforlife.com/wp-json/\n  index_authentication_field:\n    application-passwords:\n      endpoints:\n        authorization: https://leafforlife.com/wp-admin/authorize-application.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/authentication/leaf4life-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Clinical Trials
- Oncology
- Critical Care
- Drug Development
- Life Sciences
- Rare Disease
- content-api
---
