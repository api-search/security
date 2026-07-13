---
api_key_in: []
api_specs:
- filename: reference
  format: yaml
  label: WP Engine Hosting Platform API
  slug: wpengine-hosting-platform-api
  spec_type: OpenAPI
  url: https://developers.wpengine.com/docs/managed-hosting-platform/api/reference
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wpengine Authentication
name_suffix: Authentication
oauth_flows: []
overview: WP Engine secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WP Engine
provider_slug: wpengine
scheme_count: 1
schemes:
- description: 'API username and password from Portal''s API Access page: https://my.wpengine.com/api_access'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wpengine-hosting-platform-api-openapi.json
  type: http
slug: wpengine-authentication
source_filename: wpengine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wpengine-hosting-platform-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'API username and password from Portal''s API Access page: https://my.wpengine.com/api_access'\n  sources:\n  - openapi/wpengine-hosting-platform-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/authentication/wpengine-authentication.yml
summary_line: http · 1 scheme
tags:
- WordPress
- Managed Hosting
- WordPress Hosting
- Site Management
- Digital Experience Platform
---
