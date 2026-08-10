---
api_key_in: []
api_specs:
- filename: skydance-media-categories-api-openapi.yml
  format: yaml
  label: Skydance Media Categories API
  slug: skydance-media-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-categories-api-openapi.yml
- filename: skydance-media-comments-api-openapi.yml
  format: yaml
  label: Skydance Media Comments API
  slug: skydance-media-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-comments-api-openapi.yml
- filename: skydance-media-media-api-openapi.yml
  format: yaml
  label: Skydance Media Media API
  slug: skydance-media-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-media-api-openapi.yml
- filename: skydance-media-pages-api-openapi.yml
  format: yaml
  label: Skydance Media Pages API
  slug: skydance-media-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-pages-api-openapi.yml
- filename: skydance-media-posts-api-openapi.yml
  format: yaml
  label: Skydance Media Posts API
  slug: skydance-media-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-posts-api-openapi.yml
- filename: skydance-media-search-api-openapi.yml
  format: yaml
  label: Skydance Media Search API
  slug: skydance-media-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-search-api-openapi.yml
- filename: skydance-media-settings-api-openapi.yml
  format: yaml
  label: Skydance Media Settings API
  slug: skydance-media-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-settings-api-openapi.yml
- filename: skydance-media-statuses-api-openapi.yml
  format: yaml
  label: Skydance Media Statuses API
  slug: skydance-media-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-statuses-api-openapi.yml
- filename: skydance-media-tags-api-openapi.yml
  format: yaml
  label: Skydance Media Tags API
  slug: skydance-media-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-tags-api-openapi.yml
- filename: skydance-media-taxonomies-api-openapi.yml
  format: yaml
  label: Skydance Media Taxonomies API
  slug: skydance-media-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-taxonomies-api-openapi.yml
- filename: skydance-media-types-api-openapi.yml
  format: yaml
  label: Skydance Media Types API
  slug: skydance-media-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-types-api-openapi.yml
- filename: skydance-media-users-api-openapi.yml
  format: yaml
  label: Skydance Media Users API
  slug: skydance-media-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Skydance Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skydance Media secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skydance Media
provider_slug: skydance-media
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. Read operations on wp/v2 are anonymous; every write requires credentials issued from the skydance.com WordPress admin.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/skydance-media-content-openapi.yml
  type: http
slug: skydance-media-authentication
source_filename: skydance-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/skydance-media-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Read operations on wp/v2 are\n    anonymous; every write requires credentials issued from the skydance.com WordPress admin.\n  sources:\n  - openapi/skydance-media-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/authentication/skydance-media-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Entertainment
- Media
- Film
- Television
- Animation
- Video Games
- Sports
- Content
- WordPress
---
