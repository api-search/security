---
api_key_in:
- cookie
api_specs:
- filename: wordpress-rest-api-openapi.yml
  format: yaml
  label: WordPress REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-rest-api-openapi.yml
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
