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
name: Cafmlane Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: cafmlane-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: cafmlane-com
provider_slug: cafmlane-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cafmlane-com-openapi.json
  type: http
slug: cafmlane-com-authentication
source_filename: cafmlane-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/cafmlane-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cafmlane-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cafmlane-com/authentication/cafmlane-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- facility-management
- cafm
- space-utilization
- asset-management
---
