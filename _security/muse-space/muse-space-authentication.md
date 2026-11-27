---
anonymous_access: false
api_key_in: []
api_specs:
- filename: muse-space-read-api-openapi.yml
  format: yaml
  label: Muse Read API
  slug: muse-space-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muse-space/openapi/muse-space-read-api-openapi.yml
- filename: muse-space-write-api-openapi.yml
  format: yaml
  label: Muse Write API
  slug: muse-space-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muse-space/openapi/muse-space-write-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Muse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Muse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Muse
provider_slug: muse-space
scheme_count: 1
schemes:
- description: An agent token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/muse-space-openapi.json
  type: http
slug: muse-space-authentication
source_filename: muse-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/muse-space-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: An agent token.\n  sources:\n  - openapi/muse-space-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/muse-space/authentication/muse-space-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Calendar
- Email
- Privacy
---
