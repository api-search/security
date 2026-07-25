---
api_key_in:
- cookie
api_specs:
- filename: wordpress-block-types-api-openapi.yml
  format: yaml
  label: WordPress Block Types API
  slug: wordpress-block-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-block-types-api-openapi.yml
- filename: wordpress-blocks-api-openapi.yml
  format: yaml
  label: WordPress Blocks API
  slug: wordpress-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-blocks-api-openapi.yml
- filename: wordpress-categories-api-openapi.yml
  format: yaml
  label: WordPress Categories API
  slug: wordpress-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-categories-api-openapi.yml
- filename: wordpress-comments-api-openapi.yml
  format: yaml
  label: WordPress Comments API
  slug: wordpress-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-comments-api-openapi.yml
- filename: wordpress-media-api-openapi.yml
  format: yaml
  label: WordPress Media API
  slug: wordpress-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-media-api-openapi.yml
- filename: wordpress-pages-api-openapi.yml
  format: yaml
  label: WordPress Pages API
  slug: wordpress-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-pages-api-openapi.yml
- filename: wordpress-plugins-api-openapi.yml
  format: yaml
  label: WordPress Plugins API
  slug: wordpress-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-plugins-api-openapi.yml
- filename: wordpress-post-types-api-openapi.yml
  format: yaml
  label: WordPress Post Types API
  slug: wordpress-post-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-post-types-api-openapi.yml
- filename: wordpress-posts-api-openapi.yml
  format: yaml
  label: WordPress Posts API
  slug: wordpress-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-posts-api-openapi.yml
- filename: wordpress-search-api-openapi.yml
  format: yaml
  label: WordPress Search API
  slug: wordpress-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-search-api-openapi.yml
- filename: wordpress-settings-api-openapi.yml
  format: yaml
  label: WordPress Settings API
  slug: wordpress-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-settings-api-openapi.yml
- filename: wordpress-tags-api-openapi.yml
  format: yaml
  label: WordPress Tags API
  slug: wordpress-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-tags-api-openapi.yml
- filename: wordpress-themes-api-openapi.yml
  format: yaml
  label: WordPress Themes API
  slug: wordpress-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-themes-api-openapi.yml
- filename: wordpress-users-api-openapi.yml
  format: yaml
  label: WordPress Users API
  slug: wordpress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wordpress Authentication
name_suffix: Authentication
oauth_flows: []
overview: WordPress secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WordPress
provider_slug: wordpress
scheme_count: 2
schemes:
- description: WordPress cookie authentication with nonce (X-WP-Nonce header required)
  in: cookie
  name: cookieAuth
  parameter: wordpress_logged_in
  sources:
  - openapi/wordpress-rest-api-openapi.yml
  type: apiKey
- description: HTTP Basic Authentication using Application Passwords (WordPress 5.6+)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wordpress-rest-api-openapi.yml
  type: http
slug: wordpress-authentication
source_filename: wordpress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wordpress-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: wordpress_logged_in\n  description: WordPress cookie authentication with nonce (X-WP-Nonce header required)\n  sources:\n  - openapi/wordpress-rest-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Application Passwords (WordPress 5.6+)\n  sources:\n  - openapi/wordpress-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/authentication/wordpress-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CMS
- Content Management
- Open Source
- WordPress
---
