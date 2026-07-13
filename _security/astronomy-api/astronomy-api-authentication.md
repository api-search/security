---
api_key_in: []
api_specs:
- filename: astronomy-api-openapi.yml
  format: yaml
  label: Astronomy API
  slug: astronomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Astronomy Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astronomy API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Astronomy API
provider_slug: astronomy-api
scheme_count: 1
schemes:
- description: 'HTTP Basic auth: username is the Application ID and password is the

    Application Secret. The client typically sends

    `Authorization: Basic base64(applicationId:applicationSecret)`.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/astronomy-api-openapi.yml
  type: http
slug: astronomy-api-authentication
source_filename: astronomy-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/astronomy-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth: username is the Application ID and password is the\n    Application Secret. The client typically sends\n    `Authorization: Basic base64(applicationId:applicationSecret)`.\n  sources:\n  - openapi/astronomy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/authentication/astronomy-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Astronomy
- Celestial Data
- Space
- Moon Phases
- Star Charts
---
