---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumen5-video-creation-api-openapi.yml
  format: yaml
  label: Lumen5 Video Creation API
  slug: lumen5-video-creation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumen5/openapi/lumen5-video-creation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lumen5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumen5 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumen5
provider_slug: lumen5
scheme_count: 1
schemes:
- description: An API key (`lm5_sk_…`) created in Lumen5, with the scopes it was given.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/lumen5.yaml
  type: http
slug: lumen5-authentication
source_filename: lumen5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/lumen5.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: An API key (`lm5_sk_…`) created in Lumen5, with the scopes it was given.\n  sources:\n  - openapi/lumen5.yaml\n"
source_yaml_url: https://artifacts.apis.io/lumen5/authentication/lumen5-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
