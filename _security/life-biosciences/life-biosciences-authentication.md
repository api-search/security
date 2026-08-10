---
api_key_in: []
api_specs:
- filename: life-biosciences-comments-api-openapi.yml
  format: yaml
  label: Life Biosciences Comments API
  slug: life-biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-comments-api-openapi.yml
- filename: life-biosciences-discovery-api-openapi.yml
  format: yaml
  label: Life Biosciences Discovery API
  slug: life-biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-discovery-api-openapi.yml
- filename: life-biosciences-media-api-openapi.yml
  format: yaml
  label: Life Biosciences Media API
  slug: life-biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-media-api-openapi.yml
- filename: life-biosciences-oembed-api-openapi.yml
  format: yaml
  label: Life Biosciences O Embed API
  slug: life-biosciences-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-oembed-api-openapi.yml
- filename: life-biosciences-pages-api-openapi.yml
  format: yaml
  label: Life Biosciences Pages API
  slug: life-biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-pages-api-openapi.yml
- filename: life-biosciences-posts-api-openapi.yml
  format: yaml
  label: Life Biosciences Posts API
  slug: life-biosciences-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-posts-api-openapi.yml
- filename: life-biosciences-search-api-openapi.yml
  format: yaml
  label: Life Biosciences Search API
  slug: life-biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-search-api-openapi.yml
- filename: life-biosciences-taxonomies-api-openapi.yml
  format: yaml
  label: Life Biosciences Taxonomies API
  slug: life-biosciences-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/openapi/life-biosciences-taxonomies-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Life Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Life Biosciences secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Life Biosciences
provider_slug: life-biosciences
scheme_count: 0
schemes: []
slug: life-biosciences-authentication
source_filename: life-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://www.lifebiosciences.com/wp-json/\napi: Life Biosciences WordPress Content API\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The read surface requires no credential of any kind. The site's own discovery document reports\n    `\"authentication\": []` — no authentication scheme is advertised — and every collection and item\n    route captured in openapi/life-biosciences-wordpress-content-openapi.yml answers HTTP 200\n    anonymously. There is no signup, no API key, no OAuth and no developer program.\nschemes: []\nanonymous_access:\n  supported: true\n  scope: >-\n    Published content only: posts (press releases), pages, media, categories, tags, comments, site\n    search, oEmbed and the type/taxonomy/status discovery endpoints.\n  evidence:\n  - {url: 'https://www.lifebiosciences.com/wp-json/wp/v2/posts?per_page=1', http_status: 200, fetched: '2026-08-04'}\n  - {url: 'https://www.lifebiosciences.com/wp-json/wp/v2/pages?per_page=1',\
  \ http_status: 200, fetched: '2026-08-04'}\n  - {url: 'https://www.lifebiosciences.com/wp-json/wp/v2/search?search=ER-100', http_status: 200, fetched: '2026-08-04'}\ngated_surface:\n  note: >-\n    WordPress core advertises write methods and privileged reads in the same discovery document, but\n    they are not available anonymously on this host and are deliberately excluded from the OpenAPI.\n    Where writes are permitted at all they use standard WordPress credentials (cookie + X-WP-Nonce\n    for same-origin, or Application Passwords over HTTP Basic) — Life Biosciences documents neither,\n    and no public credential issuance exists.\n  observed:\n  - {url: 'https://www.lifebiosciences.com/wp-json/wp/v2/users', http_status: 401, code: rest_user_cannot_view}\n  - {url: 'https://www.lifebiosciences.com/wp-json/wp-abilities/v1/abilities', http_status: 401, note: 'WordPress Abilities API present but auth-gated; agent tool schemas cannot be introspected anonymously.'}\n  accepted_headers:\n\
  \    note: Advertised via access-control-allow-headers on the REST responses.\n    headers: [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type]\ntransport:\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  artifact: security/life-biosciences-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/authentication/life-biosciences-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Longevity
- Aging
- Gene Therapy
- Ophthalmology
- Content
---
