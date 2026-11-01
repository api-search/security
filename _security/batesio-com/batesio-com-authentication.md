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
name: Batesio Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: batesio-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: batesio-com
provider_slug: batesio-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/batesio-com-openapi.json
  type: http
slug: batesio-com-authentication
source_filename: batesio-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/batesio-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/batesio-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/batesio-com/authentication/batesio-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Management
- Accounting
- SaaS
- Small Business
- File Sharing
---
