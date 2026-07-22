---
api_key_in: []
api_specs:
- filename: smartnews-marketing-openapi.json
  format: json
  label: SmartNews Marketing API
  slug: smartnews-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-marketing-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smartnews Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartNews secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartNews
provider_slug: smartnews
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/smartnews-marketing-openapi.json
  type: http
slug: smartnews-authentication
source_filename: smartnews-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/smartnews-marketing-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/smartnews-marketing-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/authentication/smartnews-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- News
- Advertising
- AdTech
- Marketing
- Media
- Campaign Management
---
