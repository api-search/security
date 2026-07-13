---
api_key_in: []
api_specs:
- filename: orkes-conductor-api.yml
  format: yaml
  label: Orkes
  slug: orkes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-conductor-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orkes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orkes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orkes
provider_slug: orkes
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/orkes-conductor-api.yml
  type: http
slug: orkes-authentication
source_filename: orkes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orkes-conductor-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/orkes-conductor-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/authentication/orkes-authentication.yml
summary_line: http · 1 scheme
tags:
- Microservices
---
