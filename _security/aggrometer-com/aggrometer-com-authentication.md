---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aggrometer-com-openapi.yml
  format: yaml
  label: Aggrometer API
  slug: aggrometer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aggrometer-com/openapi/aggrometer-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aggrometer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aggrometer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aggrometer
provider_slug: aggrometer-com
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/aggrometer-com-openapi.json
  type: http
slug: aggrometer-com-authentication
source_filename: aggrometer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aggrometer-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aggrometer-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aggrometer-com/authentication/aggrometer-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Gaming
- Data
- Analytics
- Software-as-a-Service
---
