---
api_key_in: []
api_specs:
- filename: home-depot-home-depot-api-openapi.yml
  format: yaml
  label: Home Depot API
  slug: home-depot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/home-depot/refs/heads/main/openapi/home-depot-home-depot-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Home Depot Authentication
name_suffix: Authentication
oauth_flows: []
overview: home-depot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: home-depot
provider_slug: home-depot
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/home-depot-home-depot-api-openapi.yml
  type: http
slug: home-depot-authentication
source_filename: home-depot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/home-depot-home-depot-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/home-depot-home-depot-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/home-depot/refs/heads/main/authentication/home-depot-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 100
---
