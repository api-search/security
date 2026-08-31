---
api_key_in: []
api_specs:
- filename: pathalys-pharma-posts-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Posts API
  slug: pathalys-pharma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-posts-api-openapi.yml
- filename: pathalys-pharma-pages-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Pages API
  slug: pathalys-pharma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-pages-api-openapi.yml
- filename: pathalys-pharma-media-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Media API
  slug: pathalys-pharma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-media-api-openapi.yml
- filename: pathalys-pharma-categories-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Categories API
  slug: pathalys-pharma-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-categories-api-openapi.yml
- filename: pathalys-pharma-comments-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Comments API
  slug: pathalys-pharma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-comments-api-openapi.yml
- filename: pathalys-pharma-search-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Search API
  slug: pathalys-pharma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-search-api-openapi.yml
- filename: pathalys-pharma-discovery-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Discovery API
  slug: pathalys-pharma-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-discovery-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Pathalys Pharma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pathalys Pharma declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Pathalys Pharma
provider_slug: pathalys-pharma
scheme_count: 0
schemes: []
slug: pathalys-pharma-authentication
source_filename: pathalys-pharma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://pathalys.com/wp-json/ (site index `authentication` block) plus anonymous read probes on 2026-08-26\nsummary: >-\n  Pathalys Pharma publishes no developer program, issues no API keys, and operates no OAuth server.\n  The content API described in openapi/ is the WordPress REST API on pathalys.com, whose entire read\n  surface is anonymous — every operation modelled in this repo was verified to return HTTP 200 with\n  no credentials. Authenticated access exists only for site administrators, over WordPress's own\n  mechanisms, and is not offered to third parties.\nschemes: []\nanonymous_access:\n  supported: true\n  verified: '2026-08-26'\n  note: >-\n    GET on /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags, /wp/v2/comments,\n    /wp/v2/search, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses, /oembed/1.0/embed and the site\n    index all returned 200 unauthenticated. `context=edit` is rejected\
  \ anonymously; only `view` and\n    `embed` are available.\nadministrative_authentication:\n  advertised_by_provider: true\n  source: https://pathalys.com/wp-json/\n  mechanisms:\n  - type: application-passwords\n    standard: WordPress Application Passwords (HTTP Basic over TLS)\n    authorization_endpoint: https://pathalys.com/wp-admin/authorize-application.php\n    note: >-\n      Advertised in the `authentication` member of the REST site index. This is WordPress's built-in\n      administrative credential flow for the site's own operators — not a public API program. No\n      registration, self-service signup, or developer key issuance exists.\n  - type: cookie-nonce\n    standard: WordPress cookie authentication with an X-WP-Nonce header\n    note: >-\n      Implied by the Access-Control-Allow-Headers response header, which lists Authorization and\n      X-WP-Nonce. Only usable from a logged-in browser session on pathalys.com.\ngated_operations:\n- path: /wp/v2/settings\n  method:\
  \ GET\n  status: 401\n  code: rest_forbidden\n  note: Observed 401 anonymously — confirms the site enforces auth where WordPress expects it.\n- path: /wp/v2/users\n  method: GET\n  status: 200\n  note: >-\n    Anonymously readable (WordPress default for authors of published posts). Not modelled in the\n    OpenAPI artifacts in this repo, by API Evangelist's enrichment PII guardrail.\ntransport:\n  tls: required\n  tls_version_observed: TLSv1.3\n  hsts: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/authentication/pathalys-pharma-authentication.yml
summary_line: 0 schemes
tags:
- Company
- pharmaceuticals
- biotechnology
- nephrology
- chronic-kidney-disease
- clinical-trials
- life-sciences
- content-api
---
