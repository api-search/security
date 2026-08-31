---
api_key_in: []
api_specs:
- filename: envisics-posts-api-openapi.yml
  format: yaml
  label: Envisics Posts API
  slug: envisics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-posts-api-openapi.yml
- filename: envisics-pages-api-openapi.yml
  format: yaml
  label: Envisics Pages API
  slug: envisics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-pages-api-openapi.yml
- filename: envisics-media-api-openapi.yml
  format: yaml
  label: Envisics Media API
  slug: envisics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-media-api-openapi.yml
- filename: envisics-search-api-openapi.yml
  format: yaml
  label: Envisics Search API
  slug: envisics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-search-api-openapi.yml
- filename: envisics-discovery-api-openapi.yml
  format: yaml
  label: Envisics Discovery API
  slug: envisics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-discovery-api-openapi.yml
- filename: envisics-oembed-api-openapi.yml
  format: yaml
  label: Envisics oEmbed API
  slug: envisics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-oembed-api-openapi.yml
- filename: envisics-seo-api-openapi.yml
  format: yaml
  label: Envisics SEO Metadata API
  slug: envisics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-seo-api-openapi.yml
- filename: envisics-categories-api-openapi.yml
  format: yaml
  label: Envisics Categories API
  slug: envisics-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-categories-api-openapi.yml
- filename: envisics-tags-api-openapi.yml
  format: yaml
  label: Envisics Tags API
  slug: envisics-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-tags-api-openapi.yml
- filename: envisics-users-api-openapi.yml
  format: yaml
  label: Envisics Users API
  slug: envisics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Envisics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Envisics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Envisics
provider_slug: envisics
scheme_count: 0
schemes: []
slug: envisics-authentication
source_filename: envisics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://envisics.com/wp-json/ (root `authentication` block) + live anonymous and OPTIONS probes\nnote: >-\n  Envisics publishes no developer program, no API keys and no OAuth. The entire public surface\n  documented in this repo is ANONYMOUS and READ-ONLY: every collection answers a credential-free GET\n  and advertises `Allow: GET` on the response. The only authentication mechanism the server itself\n  advertises is WordPress application passwords, whose authorization screen lives in wp-admin and is\n  for site operators, not third-party integrators. No OAuth 2.0, no OpenID Connect, no mutual TLS,\n  no API-key scheme exists anywhere on the surface — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both returned 404 on 2026-08-12. Because the OpenAPI\n  documents carry no securitySchemes (correctly — there are none on the anonymous surface), this\n  profile was written from live probes rather\
  \ than derived by\n  0-working/derive-authentication.py, which reported 0 auth profiles for this provider.\nsummary:\n  types: []\n  anonymous_read: true\n  api_key_in: []\n  oauth2_flows: []\n  scopes_published: false\nschemes: []\nanonymous_access:\n  supported: true\n  scope: read-only\n  verified:\n  - url: https://envisics.com/wp-json/wp/v2/posts?per_page=1\n    status: 200\n    allow_header: GET\n  - url: https://envisics.com/wp-json/wp/v2/pages?per_page=1\n    status: 200\n  - url: https://envisics.com/wp-json/wp/v2/media?per_page=1\n    status: 200\n  - url: https://envisics.com/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fenvisics.com%2F\n    status: 200\n  - url: https://envisics.com/wp-json/yoast/v1/get_head?url=https%3A%2F%2Fenvisics.com%2F\n    status: 200\noperator_only:\n- mechanism: WordPress application passwords\n  advertised_at: https://envisics.com/wp-json/\n  authorization_endpoint: https://envisics.com/wp-admin/authorize-application.php\n  audience: site operators\n\
  \  note: >-\n    Advertised in the REST root `authentication` block. Not a third-party integration path; no\n    registration, no self-service issuance, no documentation.\ngated_routes_observed:\n- route: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n  note: Requires authentication; excluded from the public OpenAPI documents in this repo.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/authentication/envisics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Automotive
- Augmented Reality
- Holography
- Head-Up Display
- Photonics
- Optics
- Deep Technology
- Hardware
- Advanced Manufacturing
- Content
---
