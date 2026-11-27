---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: narrador-io-account-api-openapi.yml
  format: yaml
  label: Narrador Account API
  slug: narrador-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-account-api-openapi.yml
- filename: narrador-io-narrador-files-api-openapi.yml
  format: yaml
  label: Narrador narrador files API
  slug: narrador-io-narrador-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-narrador-files-api-openapi.yml
- filename: narrador-io-narrador-x-api-openapi.yml
  format: yaml
  label: Narrador narrador X API
  slug: narrador-io-narrador-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-narrador-x-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Narrador Authentication
name_suffix: Authentication
oauth_flows: []
overview: Narrador secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Narrador
provider_slug: narrador-io
scheme_count: 2
schemes:
- description: User API key (`nrd_files_…` or `nrd_x_…`).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/narrador-io-openapi.json
  type: http
- description: Same user API key as Bearer auth.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/narrador-io-openapi.json
  type: apiKey
slug: narrador-io-authentication
source_filename: narrador-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/narrador-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: User API key (`nrd_files_…` or `nrd_x_…`).\n  sources:\n  - openapi/narrador-io-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Same user API key as Bearer auth.\n  sources:\n  - openapi/narrador-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/narrador-io/authentication/narrador-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Text-to-Speech
- Audio
- Video
- Document Conversion
- X Posts
---
