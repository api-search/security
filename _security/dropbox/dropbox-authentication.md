---
api_key_in: []
api_specs:
- filename: dropbox-openapi-original.yml
  format: yaml
  label: Dropbox API
  slug: dropbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/openapi/dropbox-openapi-original.yml
- filename: dropbox-sign-openapi-original.yml
  format: yaml
  label: Dropbox Sign API
  slug: dropbox-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/openapi/dropbox-sign-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dropbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dropbox secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dropbox
provider_slug: dropbox
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dropbox-openapi-original.yml
  - openapi/dropbox-sign-openapi-original.yml
  type: http
- description: _t__OpenApi::AUTH::API_KEY
  name: api_key
  scheme: basic
  sources:
  - openapi/dropbox-sign-openapi-original.yml
  type: http
slug: dropbox-authentication
source_filename: dropbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dropbox-openapi-original.yml, openapi/dropbox-sign-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dropbox-openapi-original.yml\n  - openapi/dropbox-sign-openapi-original.yml\n- name: api_key\n  type: http\n  scheme: basic\n  description: _t__OpenApi::AUTH::API_KEY\n  sources:\n  - openapi/dropbox-sign-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/authentication/dropbox-authentication.yml
summary_line: http · 2 schemes
tags:
- Documents
---
