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
name: Brightseed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brightseed secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brightseed
provider_slug: brightseed
scheme_count: 1
schemes:
- description: WordPress application passwords. Authorize at https://www.brightseedbio.com/wp-admin/authorize-application.php (advertised in the /wp-json/ discovery document).
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/brightseed-categories-api-openapi.yml
  - openapi/brightseed-comments-api-openapi.yml
  - openapi/brightseed-media-api-openapi.yml
  - openapi/brightseed-pages-api-openapi.yml
  - openapi/brightseed-posts-api-openapi.yml
  - openapi/brightseed-search-api-openapi.yml
  - openapi/brightseed-statuses-api-openapi.yml
  - openapi/brightseed-tags-api-openapi.yml
  - openapi/brightseed-taxonomies-api-openapi.yml
  - openapi/brightseed-types-api-openapi.yml
  - openapi/brightseed-users-api-openapi.yml
  type: http
slug: brightseed-authentication
source_filename: brightseed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/brightseed-categories-api-openapi.yml, openapi/brightseed-comments-api-openapi.yml,\n  openapi/brightseed-media-api-openapi.yml, openapi/brightseed-pages-api-openapi.yml, openapi/brightseed-posts-api-openapi.yml,\n  openapi/brightseed-search-api-openapi.yml, openapi/brightseed-statuses-api-openapi.yml, openapi/brightseed-tags-api-openapi.yml,\n  openapi/brightseed-taxonomies-api-openapi.yml, openapi/brightseed-types-api-openapi.yml, openapi/brightseed-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords. Authorize at https://www.brightseedbio.com/wp-admin/authorize-application.php\n    (advertised in the /wp-json/ discovery document).\n  sources:\n  - openapi/brightseed-categories-api-openapi.yml\n  - openapi/brightseed-comments-api-openapi.yml\n  - openapi/brightseed-media-api-openapi.yml\n  - openapi/brightseed-pages-api-openapi.yml\n\
  \  - openapi/brightseed-posts-api-openapi.yml\n  - openapi/brightseed-search-api-openapi.yml\n  - openapi/brightseed-statuses-api-openapi.yml\n  - openapi/brightseed-tags-api-openapi.yml\n  - openapi/brightseed-taxonomies-api-openapi.yml\n  - openapi/brightseed-types-api-openapi.yml\n  - openapi/brightseed-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/authentication/brightseed-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Bioactives
- Artificial Intelligence
- Life Sciences
- Nutrition
- Ingredients
- Drug Discovery
- Agrifood
- content-api
- WordPress
---
