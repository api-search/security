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
name: Dsarvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dsarvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dsarvo
provider_slug: dsarvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/dsarvo-com-openapi.json
  type: http
slug: dsarvo-com-authentication
source_filename: dsarvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dsarvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/dsarvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dsarvo-com/authentication/dsarvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Privacy
- Compliance
- Software
- Small Business
---
