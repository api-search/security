---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- content-api
- WordPress
---
