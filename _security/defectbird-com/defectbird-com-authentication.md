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
name: Defectbird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defectbird secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Defectbird
provider_slug: defectbird-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/defectbird-com-openapi.yml
  type: http
slug: defectbird-com-authentication
source_filename: defectbird-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/defectbird-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/defectbird-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/defectbird-com/authentication/defectbird-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Automotive
- Inspection
- Software
- Software-as-a-Service
- US
---
