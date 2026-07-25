---
api_key_in:
- header
api_specs:
- filename: lish-categories-api-openapi.yml
  format: yaml
  label: Lish Categories API
  slug: lish-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-categories-api-openapi.yml
- filename: lish-comments-api-openapi.yml
  format: yaml
  label: Lish Comments API
  slug: lish-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-comments-api-openapi.yml
- filename: lish-media-api-openapi.yml
  format: yaml
  label: Lish Media API
  slug: lish-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-media-api-openapi.yml
- filename: lish-pages-api-openapi.yml
  format: yaml
  label: Lish Pages API
  slug: lish-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-pages-api-openapi.yml
- filename: lish-posts-api-openapi.yml
  format: yaml
  label: Lish Posts API
  slug: lish-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-posts-api-openapi.yml
- filename: lish-search-api-openapi.yml
  format: yaml
  label: Lish Search API
  slug: lish-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-search-api-openapi.yml
- filename: lish-statuses-api-openapi.yml
  format: yaml
  label: Lish Statuses API
  slug: lish-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-statuses-api-openapi.yml
- filename: lish-tags-api-openapi.yml
  format: yaml
  label: Lish Tags API
  slug: lish-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-tags-api-openapi.yml
- filename: lish-taxonomies-api-openapi.yml
  format: yaml
  label: Lish Taxonomies API
  slug: lish-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-taxonomies-api-openapi.yml
- filename: lish-types-api-openapi.yml
  format: yaml
  label: Lish Types API
  slug: lish-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-types-api-openapi.yml
- filename: lish-users-api-openapi.yml
  format: yaml
  label: Lish Users API
  slug: lish-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lish secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lish
provider_slug: lish
scheme_count: 1
schemes:
- description: The public read surface documented here requires NO credentials — the live index reports an empty `authentication` object. Authenticated operations use a cookie plus an `X-WP-Nonce` header (same-origin), or HTTP Basic with a WordPress Application Password (`/wp/v2/users/<id>/application-passwords` is present in the live index).
  in: header
  name: anonymous
  parameter: X-WP-Nonce
  sources:
  - openapi/lish-wordpress-openapi.json
  type: apiKey
slug: lish-authentication
source_filename: lish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lish-wordpress-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: anonymous\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: The public read surface documented here requires NO credentials — the live index\n    reports an empty `authentication` object. Authenticated operations use a cookie plus an\n    `X-WP-Nonce` header (same-origin), or HTTP Basic with a WordPress Application Password (`/wp/v2/users/<id>/application-passwords`\n    is present in the live index).\n  sources:\n  - openapi/lish-wordpress-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/authentication/lish-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Catering
- Food and Beverage
- Food Delivery
- Workplace
- Corporate Services
- Content
---
