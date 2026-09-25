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
name: Perfect Day Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perfect Day secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perfect Day
provider_slug: perfect-day
scheme_count: 1
schemes:
- description: WordPress application passwords (HTTP Basic). Required for all write operations; anonymous requests to write routes return HTTP 401 rest_forbidden.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/perfect-day-categories-openapi.yml
  - openapi/perfect-day-comments-openapi.yml
  - openapi/perfect-day-leader-categories-openapi.yml
  - openapi/perfect-day-media-openapi.yml
  - openapi/perfect-day-modals-openapi.yml
  - openapi/perfect-day-news-categories-openapi.yml
  - openapi/perfect-day-news-openapi.yml
  - openapi/perfect-day-pages-openapi.yml
  - openapi/perfect-day-posts-openapi.yml
  - openapi/perfect-day-search-openapi.yml
  - openapi/perfect-day-statuses-openapi.yml
  - openapi/perfect-day-success-stories-openapi.yml
  - openapi/perfect-day-success-story-categories-openapi.yml
  - openapi/perfect-day-tags-openapi.yml
  - openapi/perfect-day-taxonomies-openapi.yml
  - openapi/perfect-day-types-openapi.yml
  type: http
slug: perfect-day-authentication
source_filename: perfect-day-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/perfect-day-categories-openapi.yml, openapi/perfect-day-comments-openapi.yml,\n  openapi/perfect-day-leader-categories-openapi.yml, openapi/perfect-day-media-openapi.yml,\n  openapi/perfect-day-modals-openapi.yml, openapi/perfect-day-news-categories-openapi.yml, openapi/perfect-day-news-openapi.yml,\n  openapi/perfect-day-pages-openapi.yml, openapi/perfect-day-posts-openapi.yml, openapi/perfect-day-search-openapi.yml,\n  openapi/perfect-day-statuses-openapi.yml, openapi/perfect-day-success-stories-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords (HTTP Basic). Required for all write operations;\n    anonymous requests to write routes return HTTP 401 rest_forbidden.\n  sources:\n  - openapi/perfect-day-categories-openapi.yml\n  - openapi/perfect-day-comments-openapi.yml\n  - openapi/perfect-day-leader-categories-openapi.yml\n\
  \  - openapi/perfect-day-media-openapi.yml\n  - openapi/perfect-day-modals-openapi.yml\n  - openapi/perfect-day-news-categories-openapi.yml\n  - openapi/perfect-day-news-openapi.yml\n  - openapi/perfect-day-pages-openapi.yml\n  - openapi/perfect-day-posts-openapi.yml\n  - openapi/perfect-day-search-openapi.yml\n  - openapi/perfect-day-statuses-openapi.yml\n  - openapi/perfect-day-success-stories-openapi.yml\n  - openapi/perfect-day-success-story-categories-openapi.yml\n  - openapi/perfect-day-tags-openapi.yml\n  - openapi/perfect-day-taxonomies-openapi.yml\n  - openapi/perfect-day-types-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfect-day/refs/heads/main/authentication/perfect-day-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Food Technology
- Precision Fermentation
- Alternative Protein
- Ingredients
- Sustainability
- Biotechnology
- Consumer Packaged Goods
- content-api
- WordPress
---
