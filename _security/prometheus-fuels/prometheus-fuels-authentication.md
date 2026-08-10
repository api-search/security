---
api_key_in: []
api_specs:
- filename: prometheus-fuels-news-articles-api-openapi.yml
  format: yaml
  label: Prometheus Fuels news-articles API
  slug: prometheus-fuels-news-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-news-articles-api-openapi.yml
- filename: prometheus-fuels-pages-api-openapi.yml
  format: yaml
  label: Prometheus Fuels pages API
  slug: prometheus-fuels-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-pages-api-openapi.yml
- filename: prometheus-fuels-posts-api-openapi.yml
  format: yaml
  label: Prometheus Fuels posts API
  slug: prometheus-fuels-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-posts-api-openapi.yml
- filename: prometheus-fuels-media-api-openapi.yml
  format: yaml
  label: Prometheus Fuels media API
  slug: prometheus-fuels-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-media-api-openapi.yml
- filename: prometheus-fuels-categories-api-openapi.yml
  format: yaml
  label: Prometheus Fuels categories API
  slug: prometheus-fuels-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-categories-api-openapi.yml
- filename: prometheus-fuels-tags-api-openapi.yml
  format: yaml
  label: Prometheus Fuels tags API
  slug: prometheus-fuels-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-tags-api-openapi.yml
- filename: prometheus-fuels-comments-api-openapi.yml
  format: yaml
  label: Prometheus Fuels comments API
  slug: prometheus-fuels-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-comments-api-openapi.yml
- filename: prometheus-fuels-users-api-openapi.yml
  format: yaml
  label: Prometheus Fuels users API
  slug: prometheus-fuels-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-users-api-openapi.yml
- filename: prometheus-fuels-search-api-openapi.yml
  format: yaml
  label: Prometheus Fuels search API
  slug: prometheus-fuels-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-search-api-openapi.yml
- filename: prometheus-fuels-taxonomies-api-openapi.yml
  format: yaml
  label: Prometheus Fuels taxonomies API
  slug: prometheus-fuels-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-taxonomies-api-openapi.yml
- filename: prometheus-fuels-types-api-openapi.yml
  format: yaml
  label: Prometheus Fuels types API
  slug: prometheus-fuels-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-types-api-openapi.yml
- filename: prometheus-fuels-statuses-api-openapi.yml
  format: yaml
  label: Prometheus Fuels statuses API
  slug: prometheus-fuels-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/openapi/prometheus-fuels-statuses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prometheus Fuels Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prometheus Fuels secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prometheus Fuels
provider_slug: prometheus-fuels
scheme_count: 1
schemes:
- authorization_url: https://prometheusfuels.ai/wp-admin/authorize-application.php
  description: WordPress application passwords, sent as HTTP Basic credentials. The live discovery document at https://prometheusfuels.ai/wp-json/ advertises `authentication.application-passwords.endpoints.authorization` = https://prometheusfuels.ai/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/prometheus-fuels-news-articles-api-openapi.yml
  - openapi/prometheus-fuels-posts-api-openapi.yml
  type: http
slug: prometheus-fuels-authentication
source_filename: prometheus-fuels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: >-\n  openapi/prometheus-fuels-*-api-openapi.yml (derived from the live route metadata at\n  https://prometheusfuels.ai/wp-json/wp/v2) + the live discovery document at\n  https://prometheusfuels.ai/wp-json/\nscope: >-\n  Prometheus Fuels publishes no product API and no developer portal, so there is no product\n  authentication model to record. This file describes the auth posture of the one machine-readable\n  surface the company operates: the WordPress REST API behind prometheusfuels.ai.\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, sent as HTTP Basic credentials. The live discovery document at\n    https://prometheusfuels.ai/wp-json/ advertises\n    `authentication.application-passwords.endpoints.authorization` =\n    https://prometheusfuels.ai/wp-admin/authorize-application.php\n  authorization_url: https://prometheusfuels.ai/wp-admin/authorize-application.php\n\
  \  sources:\n  - openapi/prometheus-fuels-news-articles-api-openapi.yml\n  - openapi/prometheus-fuels-posts-api-openapi.yml\nanonymous_access:\n  supported: true\n  verified: '2026-08-05'\n  note: >-\n    Each collection below was fetched with no credentials and returned HTTP 200 on 2026-08-05.\n  collections_200:\n  - /wp/v2/posts\n  - /wp/v2/pages\n  - /wp/v2/news-articles\n  - /wp/v2/categories\n  - /wp/v2/tags\n  - /wp/v2/media\n  - /wp/v2/comments\n  - /wp/v2/users\n  - /wp/v2/search\n  - /wp/v2/taxonomies\n  - /wp/v2/types\n  - /wp/v2/statuses\n  collections_401:\n  - path: /wp/v2/settings\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n  - path: /wp/v2/menus\n    body: '{\"code\":\"rest_cannot_view\",\"message\":\"Sorry, you are not allowed to view menus.\",\"data\":{\"status\":401}}'\n  - path: /wp/v2/themes\n    body: '{\"code\":\"rest_cannot_view_themes\",\"message\":\"Sorry, you are not allowed to view\
  \ themes.\",\"data\":{\"status\":401}}'\n  - path: /wp/v2/plugins\n    body: '{\"code\":\"rest_cannot_view_plugins\",\"message\":\"Sorry, you are not allowed to manage plugins for this site.\",\"data\":{\"status\":401}}'\n  - path: /wp-abilities/v1/abilities\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\nwrites_require_auth: true\noauth: false\noauth_note: >-\n  No OAuth 2.0 or OpenID Connect surface exists on this host. /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both returned 404 on 2026-08-05.\nrelated:\n- conventions/prometheus-fuels-conventions.yml\n- errors/prometheus-fuels-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/authentication/prometheus-fuels-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Climate Tech
- Carbon Capture
- Synthetic Fuels
- Direct Air Capture
- Energy Storage
- Content API
- WordPress
---
