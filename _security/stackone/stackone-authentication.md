---
api_key_in: []
api_specs:
- filename: stackone-openapi.yml
  format: yaml
  label: StackOne
  slug: stackone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackone/refs/heads/main/openapi/stackone-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stackone Authentication
name_suffix: Authentication
oauth_flows: []
overview: StackOne secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StackOne
provider_slug: stackone
scheme_count: 1
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/stackone-openapi.yml
  type: http
slug: stackone-authentication
source_filename: stackone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackone-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/stackone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackone/refs/heads/main/authentication/stackone-authentication.yml
summary_line: http · 1 scheme
tags:
- Integrations
- iPaaS
---
