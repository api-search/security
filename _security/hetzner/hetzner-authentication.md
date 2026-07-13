---
api_key_in: []
api_specs:
- filename: hetzner-openapi.yml
  format: yaml
  label: Hetzner Cloud API
  slug: hetzner-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hetzner/refs/heads/main/openapi/hetzner-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hetzner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hetzner secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hetzner
provider_slug: hetzner
scheme_count: 1
schemes:
- name: APIToken
  scheme: bearer
  sources:
  - openapi/hetzner-openapi.yml
  type: http
slug: hetzner-authentication
source_filename: hetzner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hetzner-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: APIToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hetzner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hetzner/refs/heads/main/authentication/hetzner-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Hosting
- DNS
- Infrastructure
- Servers
---
