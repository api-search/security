---
api_key_in: []
api_specs:
- filename: misskey-openapi.json
  format: json
  label: Misskey API
  slug: misskey
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misskey/refs/heads/main/openapi/misskey-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Misskey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Misskey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Misskey
provider_slug: misskey
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/misskey-openapi.json
  type: http
slug: misskey-authentication
source_filename: misskey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/misskey-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/misskey-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misskey/refs/heads/main/authentication/misskey-authentication.yml
summary_line: http · 1 scheme
tags:
- Open-Source
- Social Networks
- Fediverse
- ActivityPub
- Decentralized
---
