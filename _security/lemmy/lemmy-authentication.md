---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Lemmy REST API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemmy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemmy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemmy
provider_slug: lemmy
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: lemmy-authentication
source_filename: lemmy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/authentication/lemmy-authentication.yml
summary_line: http · 1 scheme
tags:
- Communities
- Federated
- Fediverse
- Link Aggregator
- Open-Source
- Social Networks
---
