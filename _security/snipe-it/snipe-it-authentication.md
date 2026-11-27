---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snipe-it-file-api-openapi.yml
  format: yaml
  label: Snipe-IT File API
  slug: snipe-it-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-file-api-openapi.yml
- filename: snipe-it-files-api-openapi.yml
  format: yaml
  label: Snipe-IT Files API
  slug: snipe-it-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-files-api-openapi.yml
- filename: snipe-it-hardware-api-openapi.yml
  format: yaml
  label: Snipe-IT Hardware API
  slug: snipe-it-hardware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-hardware-api-openapi.yml
- filename: snipe-it-models-api-openapi.yml
  format: yaml
  label: Snipe-IT Models API
  slug: snipe-it-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-models-api-openapi.yml
- filename: snipe-it-snipe-it-api-api-openapi.yml
  format: yaml
  label: Snipe-IT Snipe IT API
  slug: snipe-it-snipe-it-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-snipe-it-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Snipe-IT Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snipe-IT secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snipe-IT
provider_slug: snipe-it
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/snipe-it-file-api-openapi.yml
  - openapi/snipe-it-files-api-openapi.yml
  - openapi/snipe-it-hardware-api-openapi.yml
  - openapi/snipe-it-models-api-openapi.yml
  - openapi/snipe-it-snipe-it-api-api-openapi.yml
  type: http
slug: snipe-it-authentication
source_filename: snipe-it-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/snipe-it-file-api-openapi.yml, openapi/snipe-it-files-api-openapi.yml, openapi/snipe-it-hardware-api-openapi.yml,\n  openapi/snipe-it-models-api-openapi.yml, openapi/snipe-it-snipe-it-api-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/snipe-it-file-api-openapi.yml\n  - openapi/snipe-it-files-api-openapi.yml\n  - openapi/snipe-it-hardware-api-openapi.yml\n  - openapi/snipe-it-models-api-openapi.yml\n  - openapi/snipe-it-snipe-it-api-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/snipe-it/authentication/snipe-it-authentication.yml
summary_line: http · 1 scheme
tags:
- IT Asset Management
- Open Source
- Cloud Hosting
- REST API
- Security
- Support
- Software
---
