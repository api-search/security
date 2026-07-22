---
api_key_in: []
api_specs:
- filename: sidequest-openapi.json
  format: json
  label: SideQuest Public API
  slug: sidequest-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sidequest Authentication
name_suffix: Authentication
oauth_flows: []
overview: SideQuest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SideQuest
provider_slug: sidequest
scheme_count: 1
schemes:
- name: userAuth
  scheme: bearer
  sources:
  - openapi/sidequest-openapi.json
  type: http
slug: sidequest-authentication
source_filename: sidequest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sidequest-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: userAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sidequest-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/authentication/sidequest-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Virtual Reality
- VR
- XR
- Gaming
- App Store
- Developers
---
