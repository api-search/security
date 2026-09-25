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
name: Legendary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Legendary Entertainment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Legendary Entertainment
provider_slug: legendary
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://www.legendary.com/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/legendary-wp-rest-openapi.yml
  type: http
slug: legendary-authentication
source_filename: legendary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/legendary-wp-rest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://www.legendary.com/wp-admin/authorize-application.php\n  sources:\n  - openapi/legendary-wp-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legendary/refs/heads/main/authentication/legendary-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Media
- Entertainment
- Film
- Television
- Comics
- Content
- Publishing
- WordPress
---
