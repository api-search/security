---
api_key_in: []
api_specs:
- filename: elixir-medical-categories-api-openapi.yml
  format: yaml
  label: Elixir Medical Categories API
  slug: elixir-medical-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-categories-api-openapi.yml
- filename: elixir-medical-comments-api-openapi.yml
  format: yaml
  label: Elixir Medical Comments API
  slug: elixir-medical-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-comments-api-openapi.yml
- filename: elixir-medical-media-api-openapi.yml
  format: yaml
  label: Elixir Medical Media API
  slug: elixir-medical-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-media-api-openapi.yml
- filename: elixir-medical-pages-api-openapi.yml
  format: yaml
  label: Elixir Medical Pages API
  slug: elixir-medical-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-pages-api-openapi.yml
- filename: elixir-medical-posts-api-openapi.yml
  format: yaml
  label: Elixir Medical Posts API
  slug: elixir-medical-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-posts-api-openapi.yml
- filename: elixir-medical-search-api-openapi.yml
  format: yaml
  label: Elixir Medical Search API
  slug: elixir-medical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-search-api-openapi.yml
- filename: elixir-medical-statuses-api-openapi.yml
  format: yaml
  label: Elixir Medical Statuses API
  slug: elixir-medical-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-statuses-api-openapi.yml
- filename: elixir-medical-tags-api-openapi.yml
  format: yaml
  label: Elixir Medical Tags API
  slug: elixir-medical-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-tags-api-openapi.yml
- filename: elixir-medical-taxonomies-api-openapi.yml
  format: yaml
  label: Elixir Medical Taxonomies API
  slug: elixir-medical-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-taxonomies-api-openapi.yml
- filename: elixir-medical-types-api-openapi.yml
  format: yaml
  label: Elixir Medical Types API
  slug: elixir-medical-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-types-api-openapi.yml
- filename: elixir-medical-users-api-openapi.yml
  format: yaml
  label: Elixir Medical Users API
  slug: elixir-medical-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-users-api-openapi.yml
- filename: elixir-medical-wpfm-designations-api-openapi.yml
  format: yaml
  label: Elixir Medical Wpfm Designations API
  slug: elixir-medical-wpfm-designations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-wpfm-designations-api-openapi.yml
- filename: elixir-medical-wpfm-locations-api-openapi.yml
  format: yaml
  label: Elixir Medical Wpfm Locations API
  slug: elixir-medical-wpfm-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-wpfm-locations-api-openapi.yml
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
method: probed
name: Elixir Medical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elixir Medical secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elixir Medical
provider_slug: elixir-medical
scheme_count: 2
schemes:
- description: Read operations on the wp/v2 content collections answer with no credential at all. Observed live on posts, pages, media, categories, users, types and taxonomies.
  name: anonymous
  sources:
  - https://elixirmedical.com/wp-json/wp/v2/posts
  type: none
- authorization_endpoint: https://elixirmedical.com/wp-admin/authorize-application.php
  description: WordPress application passwords, sent as HTTP Basic. The site's discovery document declares the authorization endpoint under `authentication.application-passwords`.
  name: applicationPassword
  scheme: basic
  sources:
  - https://elixirmedical.com/wp-json/
  - openapi/elixir-medical-wordpress-content-openapi.yml
  type: http
slug: elixir-medical-authentication
source_filename: elixir-medical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://elixirmedical.com/wp-json/\nnote: >-\n  Elixir Medical publishes no developer authentication documentation, because it runs no\n  developer program. This profile was assembled from the site's own WordPress REST discovery\n  document (which declares its authentication block) plus live anonymous probes of the\n  wp/v2 content routes. Every value below was observed, not assumed.\nsummary:\n  types:\n  - http\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    Read operations on the wp/v2 content collections answer with no credential at all.\n    Observed live on posts, pages, media, categories, users, types and taxonomies.\n  sources:\n  - https://elixirmedical.com/wp-json/wp/v2/posts\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, sent as HTTP Basic. The site's discovery\
  \ document\n    declares the authorization endpoint under `authentication.application-passwords`.\n  authorization_endpoint: https://elixirmedical.com/wp-admin/authorize-application.php\n  sources:\n  - https://elixirmedical.com/wp-json/\n  - openapi/elixir-medical-wordpress-content-openapi.yml\nobservations:\n- url: https://elixirmedical.com/wp-json/wp/v2/posts?per_page=1\n  status: 200\n  finding: anonymous read allowed\n- url: https://elixirmedical.com/wp-json/wp/v2/users\n  status: 200\n  finding: >-\n    author list is readable anonymously (WordPress default). Six author records are exposed.\n    Recorded as an observation only; no user data is stored in this repository.\n- url: https://elixirmedical.com/wp-json/wp/v2/settings\n  status: 401\n  finding: 'privileged route rejects anonymous callers with code `rest_forbidden`'\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/authentication/elixir-medical-authentication.yml
summary_line: http/none · 2 schemes
tags:
- Company
- Medical Devices
- Health
- Cardiovascular
- Coronary Intervention
- Implants
- Life Sciences
- Content
- WordPress
---
