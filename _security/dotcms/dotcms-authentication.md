---
api_key_in: []
api_specs:
- filename: dotcms-openapi.yml
  format: yaml
  label: dotCMS REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/openapi/dotcms-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dotcms Authentication
name_suffix: Authentication
oauth_flows: []
overview: dotCMS secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: dotCMS
provider_slug: dotcms
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dotcms-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/dotcms-openapi.yml
  type: http
slug: dotcms-authentication
source_filename: dotcms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dotcms-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dotcms-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dotcms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/authentication/dotcms-authentication.yml
summary_line: http · 2 schemes
tags:
- CMS
- Content
- Content Management
---
