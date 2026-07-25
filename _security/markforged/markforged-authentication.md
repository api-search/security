---
api_key_in: []
api_specs:
- filename: markforged-builds-api-openapi.yml
  format: yaml
  label: Markforged Builds API
  slug: markforged-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-builds-api-openapi.yml
- filename: markforged-devices-api-openapi.yml
  format: yaml
  label: Markforged Devices API
  slug: markforged-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-devices-api-openapi.yml
- filename: markforged-organizations-api-openapi.yml
  format: yaml
  label: Markforged Organizations API
  slug: markforged-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-organizations-api-openapi.yml
- filename: markforged-parts-api-openapi.yml
  format: yaml
  label: Markforged Parts API
  slug: markforged-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-parts-api-openapi.yml
- filename: markforged-print-jobs-api-openapi.yml
  format: yaml
  label: Markforged Print Jobs API
  slug: markforged-print-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-print-jobs-api-openapi.yml
- filename: markforged-printed-parts-api-openapi.yml
  format: yaml
  label: Markforged Printed Parts API
  slug: markforged-printed-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-printed-parts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Markforged Authentication
name_suffix: Authentication
oauth_flows: []
overview: Markforged secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Markforged
provider_slug: markforged
scheme_count: 1
schemes:
- description: HTTP Basic Auth using an Eiger Access Key as the username and Secret Key as the password, generated from the Eiger organization settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/markforged-openapi.yml
  type: http
slug: markforged-authentication
source_filename: markforged-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/markforged-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using an Eiger Access Key as the username and Secret Key as the\n    password, generated from the Eiger organization settings.\n  sources:\n  - openapi/markforged-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/authentication/markforged-authentication.yml
summary_line: http · 1 scheme
tags:
- 3D Printing
- Additive Manufacturing
- Industrial
- Eiger
- Fleet Management
---
