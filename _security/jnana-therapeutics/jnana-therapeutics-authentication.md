---
api_key_in: []
api_specs:
- filename: jnana-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Comments API
  slug: jnana-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-comments-api-openapi.yml
- filename: jnana-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Discovery API
  slug: jnana-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-discovery-api-openapi.yml
- filename: jnana-therapeutics-media-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Media API
  slug: jnana-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-media-api-openapi.yml
- filename: jnana-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Oembed API
  slug: jnana-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-oembed-api-openapi.yml
- filename: jnana-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Pages API
  slug: jnana-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-pages-api-openapi.yml
- filename: jnana-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Posts API
  slug: jnana-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-posts-api-openapi.yml
- filename: jnana-therapeutics-search-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Search API
  slug: jnana-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-search-api-openapi.yml
- filename: jnana-therapeutics-seo-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Seo API
  slug: jnana-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-seo-api-openapi.yml
- filename: jnana-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Taxonomy API
  slug: jnana-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-taxonomy-api-openapi.yml
- filename: jnana-therapeutics-team-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Team API
  slug: jnana-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-team-api-openapi.yml
- filename: jnana-therapeutics-theme-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Theme API
  slug: jnana-therapeutics-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-theme-api-openapi.yml
- filename: jnana-therapeutics-users-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Users API
  slug: jnana-therapeutics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Jnana Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jnana Therapeutics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Jnana Therapeutics
provider_slug: jnana-therapeutics
scheme_count: 2
schemes:
- applies_to: All operations in openapi/jnana-therapeutics-content-openapi.yml. Every one of the 25 derived operations returned 200 with no credential on 2026-08-23.
  id: anonymous
  notes: '`context=view` (the default) is anonymous. `context=edit` requires an authenticated session and returns 401 rest_forbidden without one.'
  status: in-use
  type: none
- advertised_at: https://www.jnanatx.com/wp-json/
  applies_to: Write operations and the administrative surface only. Not usable by the public — an account on the WordPress install is required, and no self-service registration is offered.
  authorization_endpoint: https://www.jnanatx.com/wp-admin/authorize-application.php
  id: application-passwords
  notes: Declared verbatim in the REST index as authentication.application-passwords.endpoints.authorization. WordPress Application Passwords are transmitted as HTTP Basic credentials over TLS.
  scheme: basic
  status: advertised
  type: http
slug: jnana-therapeutics-authentication
source_filename: jnana-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://www.jnanatx.com/wp-json/ (route index `authentication` block) plus live anonymous\n  and OPTIONS probes of the wp/v2 surface on 2026-08-23; contract shape defined upstream at\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary: >-\n  Jnana Therapeutics publishes no developer authentication documentation, because it publishes no\n  developer program. The WordPress REST content API behind www.jnanatx.com is anonymously readable\n  for its published-content routes and requires a WordPress account for everything else. The only\n  credential mechanism the deployment advertises is WordPress Application Passwords, whose\n  authorization endpoint is named in the REST index.\nsecurity_schemes: []\nschemes:\n- id: anonymous\n  type: none\n  status: in-use\n  applies_to: >-\n    All operations in openapi/jnana-therapeutics-content-openapi.yml.\
  \ Every one of the 25 derived\n    operations returned 200 with no credential on 2026-08-23.\n  notes: >-\n    `context=view` (the default) is anonymous. `context=edit` requires an authenticated session and\n    returns 401 rest_forbidden without one.\n- id: application-passwords\n  type: http\n  scheme: basic\n  status: advertised\n  advertised_at: https://www.jnanatx.com/wp-json/\n  authorization_endpoint: https://www.jnanatx.com/wp-admin/authorize-application.php\n  applies_to: >-\n    Write operations and the administrative surface only. Not usable by the public — an account on\n    the WordPress install is required, and no self-service registration is offered.\n  notes: >-\n    Declared verbatim in the REST index as\n    authentication.application-passwords.endpoints.authorization. WordPress Application Passwords\n    are transmitted as HTTP Basic credentials over TLS.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nanonymous_read: true\nwrite_surface_anonymous:\
  \ false\nevidence:\n- url: https://www.jnanatx.com/wp-json/wp/v2/posts?per_page=1\n  method: GET\n  status: 200\n  note: Anonymous read succeeds.\n- url: https://www.jnanatx.com/wp-json/wp/v2/posts\n  method: OPTIONS\n  status: 200\n  note: '`allow: GET` — no write method is offered to an anonymous caller.'\n- url: https://www.jnanatx.com/wp-json/wp/v2/settings\n  method: GET\n  status: 401\n  note: 'rest_forbidden — \"Sorry, you are not allowed to do that.\"'\n- url: https://www.jnanatx.com/wp-json/wp-abilities/v1/abilities\n  method: GET\n  status: 401\n  note: rest_forbidden.\n- url: https://www.jnanatx.com/wp-json/contact-form-7/v1/contact-forms\n  method: GET\n  status: 403\n  note: wpcf7_forbidden.\n- url: https://www.jnanatx.com/wp-json/wp/v2/menu-items\n  method: GET\n  status: 401\n  note: rest_cannot_view.\ntransport:\n  https_only: true\n  hsts: 'max-age=63072000; includeSubDomains; preload'\n  tls_version: TLSv1.3\n  cors:\n    access_control_allow_headers: 'Authorization,\
  \ X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'\n    access_control_expose_headers: 'X-WP-Total, X-WP-TotalPages, Link'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/authentication/jnana-therapeutics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Chemoproteomics
- Rare Disease
- Immunology
- Life Sciences
- Clinical Trials
- content-api
---
