---
api_key_in: []
api_specs:
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Devices API
  slug: eiger-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Builds API
  slug: eiger-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Print Jobs API
  slug: eiger-print-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Parts API
  slug: eiger-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Printed Parts API
  slug: eiger-printed-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Organizations API
  slug: eiger-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
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
